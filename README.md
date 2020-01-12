[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen.svg)](LICENSE)

# kolektif

`kolektif` is an open-source web application to help people manage events and special-interest groups.

## Prerequisites

The only prerequisites is JDK 11. Gradle (build tool) will be downloaded and setup on first run.

## Setup Steps

The application can be built and run via different methods:

- Gradle for development, and
- All-in-one JAR for distribution 

Following any of the above method will allow the application to be accessible from [`localhost:8080`](http://localhost:8080) from your browser.

### Development mode via Gradle

  1. Run `./gradlew bootRun` to start the application in development mode

### All-in-One JAR

  1. Run `./gradlew bootJar` to build an all-in-one JAR for the web application
  2. Run `java -jar build/libs/*-all.jar` to run the application

Now you can visit it on [`localhost:8080`](http://localhost:8080) from your browser.

## Code Formatting

We follow [Google Java styleguide] for code formatting and style.

  - Import the relevant configuration to your favourite IDE to auto-apply formatting during development time, or
  - Run `spotlessCheck` and `spotlessApply` prior to committing your code to apply auto-formatting

We also specify a particular import order (as defined within the Gradle's `spotless` configuration):

  1. `java`
  2. `javax`
  3. Any other namespaces
  4. Any other static namespaces
  4. `com.hhandoko`
  5. Static `com.hhandoko`

## Contributing

We follow the "[feature-branch]" Git workflow.

  1. Commit changes to a branch in your fork (use `snake_case` convention):
     - For technical chores, use `chore/` prefix followed by the short description, e.g. `chore/do_this_chore`
     - For new features, use `feature/` prefix followed by the feature name, e.g. `feature/feature_name`
     - For bug fixes, use `bug/` prefix followed by the short description, e.g. `bug/fix_this_bug`
  1. Rebase or merge from "upstream"
  1. Submit a PR "upstream" to `develop` branch with your changes

Please read [CONTRIBUTING] for more details.

## License

```
    Copyright (c) 2020 kolektif Contributors

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
```

`kolektif` is released under the Apache Version 2.0 License. See the [LICENSE] file for further details.

[CONTRIBUTING]: https://github.com/hhandoko/kolektif/blob/master/CONTRIBUTING.md
[feature-branch]: http://nvie.com/posts/a-successful-git-branching-model/
[Google Java styleguide]: https://google.github.io/styleguide/javaguide.html
[LICENSE]: https://github.com/hhandoko/kolektif/blob/master/LICENSE.txt
