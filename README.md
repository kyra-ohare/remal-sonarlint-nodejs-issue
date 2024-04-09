This repo is to demo an issue coming from Remal sonarlint by which I cannot tell the plugin to ignore `html` files.

Remal documentation: https://github.com/remal-gradle-plugins/sonarlint/blob/main/README.md


To reproduce the error, run `./gradlew clean build` and observe the logs where it says:
```log
Error while running Node.js. A supported version of Node.js is required for running the analysis of JS in HTML files. Please make sure a supported version of Node.js is available in the PATH. Alternatively, you can exclude JS in HTML files from your analysis using the 'sonar.exclusions' configuration property. See the docs for configuring the analysis environment: https://docs.sonarsource.com/sonarqube/latest/analyzing-source-code/languages/javascript-typescript-css/
```

A number of attempts were given. Please see [build.gradle](./build.gradle) line 29.
