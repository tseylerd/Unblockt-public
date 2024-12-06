![Version Badge](https://img.shields.io/badge/version-0.0.1-red)
![License Badge](https://img.shields.io/badge/license-PolyForm_Perimeter_License_1.0.0-green)

<div align=left>
  <picture>
    <source width="128" height="128" media="(prefers-color-scheme: dark)" srcset="images/logo/whiteLogo.png">
    <source width="128" height="128" media="(prefers-color-scheme: light)" srcset="images/logo/blackLogo.png">
    <img width="128" height="128" alt="logo" src="images/logo/blackLogo.png">
  </picture>
</div>

# Unblockt

### Kotlin language support for Visual Studio Code
This repository serves as a hub for documentation and feedback. Please use [GitHub Issues](https://github.com/tseylerd/Unblockt-public/issues) to share your feedback. 

**Note:** This extension is in its early stages and does not yet support all build systems or Kotlin features.
Currently:
- Projects need to use Gradle as the build system.
- Projects should follow the basic Gradle directory layout.
- The extension works best with small projects and may be unstable or perform poorly on relatively big projects.
- For more details, see the [limitations](#limitations) section.

Your feedback is invaluable—please [report](https://github.com/tseylerd/Unblockt-public/issues) any issues you encounter.
## Installation
1. Install the `Unblockt` extension from the Visual Studio Code Marketplace.
2. Open any `.kt` or `.kts` file to activate the extension.

Upon activation, the extension will:
- Launch the language server
- Read the project structure using Gradle
- Index project files to enable code insight features

Once indexing is complete, you're ready to code!

## Basics
- **Memory Widget:** A widget in the bottom right corner displays current memory usage.  
  ![Memory widget](images/ui/memoryWidget.png)
- **Unblockt Actions:** Click the widget to access a list of actions.

## Requirements
- **Java**
- **Memory:** Minimum 4GB, 8GB recommended

## Settings
- **Memory:** Configure the language server's heap size (in MB). Restart required.  
  ![Memory settings](images/ui/memorySettings.png)

## Features
- **Semantic Highlighting**  
  ![Semantic highlighting](images/code/highlighting.png)
- **Code Completion**  
  ![Code completion](images/code/codeCompletion.gif)
- **Go to Definition**  
  ![Go to definition](images/code/goToDefinition.gif)

## Actions
- **Reload Gradle Project:** Updates project structure from Gradle and applies changes.
- **Rebuild Indexes:** Clears and rebuilds project indexes.

## Limitations
- Only Gradle projects are supported.
- Only the basic Gradle directory layout is supported:
  - The `main` and `test` source sets must be located inside the `src` directory of the module.

  **Example of a supported layout:**
  ```
  <project-root>
  └── src
      ├── main
      │   ├── java
      │   │   └── <source files>
      │   └── kotlin
      │       └── <source files>
      └── test
          ├── java
          │   └── <test source files>
          └── kotlin
              └── <test source files>
  ```
- Code analysis is supported only for Kotlin code targeting the JVM.
- Code analysis for Gradle build scripts is not available.
- The extension works best with small projects and may be unstable or perform poorly on relatively big projects. Please report any performance issues encountered.

## Roadmap
Future features will depend on user feedback. Currently planned:
- Find Usages
- Rename Refactoring
- Kotlin Multiplatform Support
- Standalone Language Server

## Feedback
Please, use [GitHub Issues](https://github.com/tseylerd/Unblockt-public/issues) to report any feedback.

## Our Goal
We want developers to enjoy working with Kotlin without having to change their habits.  
To achieve this, we aim to create another high-quality tool for Kotlin development, including a standalone Language Server implementation.

## Open source software used
- [Kotlin](https://github.com/JetBrains/kotlin)
- [IntelliJ IDEA Community Edition](https://github.com/JetBrains/intellij-community)
- [MapDB](https://github.com/jankotek/mapdb)
- [Caffeine](https://github.com/ben-manes/caffeine)
- [lz4java](https://github.com/lz4/lz4-java)
- [DefinitelyTyped](https://github.com/DefinitelyTyped/DefinitelyTyped)
- [esbuild](https://github.com/evanw/esbuild)
- [Gradle Tooling](https://github.com/gradle/gradle)
- [Log4j2](https://github.com/apache/logging-log4j2)
- [System Stubs](https://github.com/webcompere/system-stubs)
- [vscode-languageserver-node](https://github.com/Microsoft/vscode-languageserver-node)