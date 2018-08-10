# What is SpecFlow?

- Open source tool for "bridging the communication gap between domain experts and developers"
- Allows non-technical people to write acceptance tests for a system
- Enabled these acceptance tests to be automated and the acceptance tests "executed" against the system
- Project site: http://www.specflow.org

## What is an acceptance test?

- Validates that the right system is built
- Business/user/customer point of view or a product owner
- Written in non-technical format, should be easy to understand format
- The result is determined as *Pass/Fail*
- Helps document what the system should do
- When automated, become "living documentation"
- Usually execute a vertical slice through the system
- Shared team understanding of what's being built
- Helps define what "done" means

By automating acceptance tests we create a link between the specification and the actual implementation.

## What is Gherkin?

- Business readable domain specific language
- Represents tests in natural language, not code
- Line-oriented
- Uses indentation to create structure
- Keywords (e.g. Feature, Scenerio)
- Localised in 40+ spoken language

### Features
- Features are the top level grouping in Gherkin.
- A feature contains one or more scenerios.

```md
Feature: Calculator

Scenario Outline: Add two numbers
    Given I have entered a into the calculator 
    And I have entered b into the calculator 
    When I press add
    Then the result should be <result> on the screen 
```

#### Format to use
- As a... I want... So that...

### Background

- Provides context (state setup) to the scenarios in a feature
- Executed before every scenario

```md
Background:
	Given I have teeth
	And I have some toothpaste

Scenario: Successful brushing
...

Scenario: Toothpaste runs out
...
```

### Coding the automation steps

- Install Specflow from Extension and Updates

Install the Nuget package:

```bash
$> Specflow.NUnit
```

> This will also install NUNit and Specflow to the project.

