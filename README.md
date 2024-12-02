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
**Note:** This extension is in its early stages. Your feedback is invaluable—please [report](https://github.com/tseylerd/Unblockt-public/issues) any issues you encounter.

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
- Only the standard Gradle file layout is supported.
- Only Kotlin JVM target is supported.
- Code insight for Gradle scripts is not yet available.

## Roadmap
Future features will depend on user feedback. Currently planned:
- Find Usages
- Rename Refactoring
- Kotlin Multiplatform Support

## Open source software used
- [Kotlin](https://github.com/JetBrains/kotlin)
- [IntelliJ IDEA Community Edition](https://github.com/JetBrains/intellij-community)
- [Caffeine](https://github.com/ben-manes/caffeine)
- [DefinitelyTyped](https://github.com/DefinitelyTyped/DefinitelyTyped)
- [esbuild](https://github.com/evanw/esbuild)
- [Gradle Tooling](https://github.com/gradle/gradle)
- [Log4j2](https://github.com/apache/logging-log4j2)
- [Sqlite JDBC](https://github.com/xerial/sqlite-jdbc)
- [System Stubs](https://github.com/webcompere/system-stubs)
- [vscode-languageserver-node](https://github.com/Microsoft/vscode-languageserver-node)