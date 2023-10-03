# Solutions Maven Build Onboarding

The purpose of this project is to learn how to improve Maven builds with Gradle Enterprise.
We've set this up to have commonly encountered build issues.
The full list of build issues this project has is written below.

Your starting point is the `main` branch. Ensure any GE extension configuration is applied only to the modules where it is required. Good luck! :)

## List of issues

When resolving the following issues, ensure the GE extension configuration is applied only to the modules where it is required.

* Caching not configured for goals that should be made cacheable
* System property used test goal, but not configured as an input, causing caching to be disabled
* Volatile goal inputs
* Absolute paths as goal inputs
* Undeclared file input to test goal
* GE configuration in a submodule that requires setting an appropriate pom.xml merge strategy

## Disclaimers

* Forked from the [spring-data-cassandra project](https://github.com/spring-projects/spring-data-cassandra) and modified for our needs
* [Original README](README_ORIGINAL.md)
* [Apache License](LICENSE.txt)

## Branches

* [main](https://github.com/gradle/gradle-enterprise-solutions-maven-onboarding) - ([changes](https://github.com/gradle/ge-solutions-onboarding-maven/compare/onboarding-repo-base...main)), which is set up with all the problems
* [onboarding-setup-fixes](https://github.com/gradle/gradle-enterprise-solutions-maven-onboarding/tree/onboarding-setup-fixes) - ([changes](https://github.com/gradle/gradle-enterprise-solutions-maven-onboarding/compare/onboarding-setup-fixes)), which fixes all the problems
* [onboarding-ge-solutions](https://github.com/gradle/gradle-enterprise-solutions-maven-onboarding/tree/onboarding-ge-solutions) - ([changes](https://github.com/gradle/gradle-enterprise-solutions-maven-onboarding/compare/onboarding-ge-solutions)), follows the `main` branch but has a basic GE setup for the [Solutions GE instance](https://ge.solutions-team.gradle.com/scans)

## Contributing

When adding/modifying this project to include new issues, you should:

- Update the readme by specifying what problem was added in the `List of issues`, as well as in the `Branches` part specifying
  on which branch it was added or if a new branch was added and what was done there.
- After your changes are merged to `main`, you should merge `main` into [onboarding-ge-solutions](https://github.com/gradle/gradle-enterprise-solutions-maven-onboarding/tree/onboarding-ge-solutions) and
  [onboarding-setup-fixes](https://github.com/gradle/gradle-enterprise-solutions-maven-onboarding/tree/onboarding-setup-fixes)
- You should implement a fix of the new issue on the branch [onboarding-setup-fixes](https://github.com/gradle/gradle-enterprise-solutions-maven-onboarding/tree/onboarding-setup-fixes).