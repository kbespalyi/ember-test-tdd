# ember-test-tdd

This README outlines the details of collaborating on this Ember application.
A short introduction of this app could easily go here.

## Prerequisites

You will need the following things properly installed on your computer.

* [Git](https://git-scm.com/)
* [Node.js](https://nodejs.org/) (with NPM)
* [Bower](https://bower.io/)
* [Ember CLI](https://ember-cli.com/)
* [PhantomJS](http://phantomjs.org/)

## Installation

* `git clone <repository-url>` this repository
* `cd ember-test-tdd`
* `npm install`
* `bower install`

## Running / Development

* `ember serve`
* Visit your app at [http://localhost:4200](http://localhost:4200).

### Code Generators

Make use of the many generators for code, try `ember help generate` for more details

### Running Tests

* `ember test`
* `ember test --server`

### Building

* `ember build` (development)
* `ember build --environment production` (production)

### Deploying

Specify what it takes to deploy your app.

## Further Reading / Useful Links

* [ember.js](http://emberjs.com/)
* [ember-cli](https://ember-cli.com/)
* Development Browser Extensions
  * [ember inspector for chrome](https://chrome.google.com/webstore/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi)
  * [ember inspector for firefox](https://addons.mozilla.org/en-US/firefox/addon/ember-inspector/)

## Annotation
Javascript TDD Is Different

When implementing TDD on the client-side, we’ll need to divide our testing mindset into client-side and server-side concerns.
Client-side JavaScript cannot query a database. It can make calls for a query or query data presented on the client-side. It cannot, however, directly fetch and insert into a database. This is important because we want to assume that the data being given to the client-side (in our tests) is gospel. We should treat the server-side data being sent as an external dependency on our test.
In many ways, we’re splitting up our applications into two contained testing areas: Server-side tests are concerned with things that go on inside the server; client-side tests are concerned with stuff that happens in the web browser. In order to achieve proper test coverage of these two aspects, the amount of tests we’re hauling along is going to increase. In some cases, we could have all of the following:
 * Client-side integration tests
 * Server-side functional tests
 * Server-side unit tests
 * Client-side unit tests
 * Client-side functional tests

Adding a lot more test weight to your application might not seem like the most attractive option. Yet, its a consequence of having complex processing on the server- and client-sides of your application. There’s a lot more space to be covered, and understanding more of what’s going on is essential!
