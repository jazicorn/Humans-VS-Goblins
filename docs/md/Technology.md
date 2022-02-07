## Technology
> References for technology used in project

Project Tools
|   Tool   |  Version  |     Purpose     | Install | Documentation |
| :------: | :-------: | :-------------: | :-----: | :-----------: |
| IntelliJ | Community | Code Editor     | [Downloads](https://www.jetbrains.com/idea/download/#section=mac) | [Resources](https://www.jetbrains.com/idea/resources/) |
| Homebrew | 1.16.1    | Package Manager | [Install](https://brew.sh/) | [Docs](https://docs.brew.sh/) |

Project Dependencies
|   Dep   |  Version  |     Purpose     | Install | Documentation |
| :-----: | :-------: | :-------------: | :-----: | :-----------: |
| Java    | 11        | Language        | [Downloads](https://www.oracle.com/java/technologies/downloads/) | [Docs](https://docs.oracle.com/en/java/javase/11/) |
| Gradle  | 7.3.3     | Build Platform  | [Install](https://gradle.org/install/) | [Docs](https://groovy-lang.org/documentation.html) |
| Groovy  | 4.0.0     | Build Script DSL| [Install](https://groovy-lang.org/install.html) | [Docs](https://docs.gradle.org/current/userguide/userguide.html) |
| Jenkins | openjdk@11| CI/CD           | [Install](https://www.jenkins.io/doc/book/installing/) | [Docs](https://www.jenkins.io/doc/) |

Project Libraries
|  Tool  | Version |  Purpose  | Documentation |
| :----: | :-----: | :-------: | :-----------: |
| JUnit  |    5    | Testing   | [Docs](https://junit.org/junit5/docs/current/user-guide/) |

### Testing
Jenkins Scripts (app)
> Default runs on http://localhost:8080 | http://127.0.0.1:8080/
```bash
brew services start jenkins
brew services stop jenkins
brew services restart jenkins
brew upgrade jenkins
```