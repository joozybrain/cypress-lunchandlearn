# README


## Lab Exercise

Run the following commands

```shell
git clone https://github.com/joozybrain/cypress-lunchandlearn
yarn install
yarn start
```
For Windows

```shell
git clone https://github.com/joozybrain/cypress-lunchandlearn
yarn install:win32
yarn start:win32
```

## How to install and use Cypress

Run the following commands

```shell
yarn add cypress
```

```shell
"scripts": {
  "test:cypress": "cypress open",           // run in browser
  "test:cypress-headless": "cypress run",   // run headless - useful in CI
}
```

```
yarn test:cypress
```
### Create a Cypress test for a user story

### Acceptance Criteria:
Given I want to sign up for an account
- When I click to sign up
- Then I should be asked to provide an email address
- And password


Given I have provided a valid email address and valid password
- When I click to create account
- Then I should get a confirmation that my account was created successfully


Given I enter an email that is already in use
- When I click to create account
- Then I should be informed that:
- "The email address you have entered is already associated with another account."


## Useful APIs

#### cy.visit(http://localhost:300);
- Indicate which web page you want to start your cypress test
#### .click()
- Simulate mouse click
#### .type()
- Simulate keyboard typing
#### .should() and .contains()
- Assertion tests to make sure your actual results and expected results are the same.
```
cy.get("#user-name").contains("Bob");

cy.get(".alert-danger").contains(/^(?!\s*$).+/);
```




