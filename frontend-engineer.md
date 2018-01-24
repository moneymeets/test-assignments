# Test assignment (frontend)

## Legend

moneymeets has developed an API to access the list of all offered investment strategies. We need to implement a web application that shows a list or a table containing all available investment strategies along with the most important properties, namely:

  * Strategy name
  * Asset manager name
  * Risk class
  * Minimum investment amount

Optionally, it would be beneficial to show the time-weighted return for the last 365 days. Since obtaining this data is very resource intensive, it is provided by a separate API endpoint. Therefore, these numbers would need to be loaded one by one.

## Deliverable

The source code for the client application should be made available to us in a  `git` repository that we can access.

## Requirements

Implement a stand-alone production-ready web application in AngularJS or Angular 2+ following best practices in the community.

Concentrate on properly setting up the project and following clean code guidelines. A project that perfectly implements only the main requirements is preferable over a quick & dirty project that implements all of the requirements. Design & UX are not the primary focus of this assignment.

### Notes

* You **may** use the Angular CLI for creating a project.
* You **may** use JavaScript or TypeScript.
* You may **not** use starter projects or project templates for AngularJS or Angular.
* API endpoints do not require authorization; documentation is available when accessing the endpoints using the browser.

#### Endpoints

  * Base endpoint:
    > [https://api.moneymeets.com/securities/v1/](https://api.moneymeets.com/securities/v1/)

  * Investment strategies endpoint:
    > [https://api.moneymeets.com/securities/v1/asset-management/investment-strategies/](https://api.moneymeets.com/securities/v1/asset-management/investment-strategies/)

  * Investment strategy's performance endpoint:
    > [https://api.moneymeets.com/securities/v1/asset-management/investment-strategies/{strategy_id}/performance](https://api.moneymeets.com/securities/v1/asset-management/investment-strategies/1/performance)
