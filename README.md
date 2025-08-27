# How This Project is Structured

- The project uses maven modules
- All module pom.xml inherit dependencies from the parent pom.xml
- Parent pom.xml should contain core dependencies like JUnit, Lombok, Logging, etc.
- Module pom.xml should add specific dependencies e.g. Project Reactor

## Courses

- This contains sub-modules to cover specific areas of interest e.g.
  - Project Reactor
  - Hibernate
  - Etc.

## Neetcode

- This contains Leetcode-like tasks
- These tasks are meant to be small, one task per file
- For the convinience of testing, tests are included in the same file as the main function code

## Samples

- This contains sub-modules with mini-projects e.g.
  - LRU Cache
  - Rate Limiter
  - Etc.
- These are meant to be slightly bigger than typical Leetcode-style tasks and go more in depth

# Common Issues

- IntelliJ says "the output path is not specified for module java-projects"
  - Go to run configuration and check the `-cp` argument. If it's `java-projects`, change it to the appropriate module