# SonarQube

An open-source platform developed by SonarSource for continuous inspection of code quality to perform automatic reviews with static analysis of code to detect bugs and code smells.

## Tools

- [SonarLint](https://www.sonarsource.com/products/sonarlint/)
- [Pair SonarLint with SonarQube](https://www.sonarqube.org/sonarlint/)

## Running Commands

- To execute code analysis, run

```console
docker run \
    --rm \
    -v "<path-to-project>:/usr/src" \
    sonarsource/sonar-scanner-cli \
    -Dsonar.projectKey=<project-key> \
    -Dsonar.host.url=http://<ip-address>:<port> \ # <ip-address> can be replaced by domain name
    -Dsonar.login=<token>
```
