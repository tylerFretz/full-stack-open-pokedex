# FullStackOpen 2020 Part 11 - CI/CD

### Points to discuss:

#### 1. Some common steps in a CI setup include linting, testing, and building. What are the specific tools for taking care of these steps in the ecosystem of the language you picked? You can search for the answers by google.

I have chosen Java as the the language this hypothical project will utilize. 

- Linting

I would generally just rely on a powerful IDE such as IntelliJ but you could use a plugin such as Checkstyle.

- Testing

JUnit for unit testing. Selenium from e2e testing. Emphasis should be placed on unit testing, as accoring to Martin Fowler

> I always argue that high-level tests are there as a second line of test defense. If you get a failure in a high level test, not just do you have a bug in your functional code, you also have a missing or incorrect unit test. Thus I advise that before fixing a bug exposed by a high level test, you should replicate the bug with a unit test. Then the unit test ensures the bug stays dead.

- Building

Gradle (used more for mobile) or Maven (used more for development).


#### 2. What alternatives are there to set up the CI besides Jenkins and GitHub Actions? Again, you can ask google!

- Atlassian Bamboo
- Bitrise
- Cruise Control
- CircleCI
- GitLab CI/CD
- Shippable
- Spinnaker
- Travis CI
- TeamCity
- UrbanCode


#### 3.  Would this setup be better in a self-hosted or a cloud-based environment? Why? What information would you need to make that decision?

A cloud-based environment would likely be preferable. However, for larger projects where more resources are needed or in larger companies where there are multiple teams and projects to take advantage of it, a self-hosted CI setup is probably the way to go.