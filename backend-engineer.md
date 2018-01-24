# Test assignment (backend)

## Legend

Our partner [figo](https://www.figo.io) provides APIs to access customer bank account information. We need to build an API client prototype to understand whether figo API works as advertised and actually fulfills our needs.

Specifically, we need to know whether (given user credentials) we can log into their system and request available bank accounts along with the corresponding metadata.

## Deliverable

The source code for the client application should be made available to us in a `git` repository that we can access.

## Requirements

Implement a stand-alone production-ready console application in a language of your choice following best practices in the corresponding community. The application should follow standard GNU tools conventions for command line interface.

### Input parameters

1. `CLIENT_ID`
2. `CLIENT_SECRET`
3. `USERNAME`
4. `PASSWORD`
5. Optional: bank account identifier

### Output format

If bank account identifier is provided, then return the balance for this bank account. Otherwise, return the list of the available bank accounts. The output should be formatted as JSON.

The only following information should be returned:

* If bank account list is requested:
    * `account_id`
    * `bank_id`
    * `jban`
    * `type`
* If account balance is requested:
    * `balance`
    * `balance_date`

N.B.: `jban` is a fictional bank account identification system, and is computed by taking every second character of the IBAN.

Example:

* `iban`: DE40900900424711951501
* `jban`: E0090271551

### Notes

* You may **not** use SDKs provided by figo
* You **may** use provided OpenAPI spec if you wish
* Demo user account credentials may not be used to obtain tokens; therefore, you **do not** need to implement the login sequence, but rather ignore provided `USERNAME` and `PASSWORD` values and use hardcoded demo user token instead.

Figo API documentation and demo access credentials are available at the following URL: [http://docs.figo.io](http://docs.figo.io).

