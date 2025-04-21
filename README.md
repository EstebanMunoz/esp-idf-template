[![Copier](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/copier-org/copier/master/img/badge/badge-grayscale-inverted-border-orange.json)](https://github.com/copier-org/copier)

# ESP-IDF Template

This is a project template built using [Copier](https://copier.readthedocs.io/) for initializing ESP SoC development projects using the [ESP-IDF framework](https://docs.espressif.com/projects/esp-idf/en/latest/). The generated project is preconfigured to allow for an initial build, enabling code completion out of the box in Zed and VS Code.

## Features

- Clean and minimal starting point
- First build support for code completion and IntelliSense
- Preconfigured ESP-IDF project structure

## Project structure

```
📁 {{project_name}}           # Your generated project
├── 📁 .git                   # Git dir
├── 📁 .vscode (optional)     # Configurations dir for VS Code
│   └── 📄 settings.json      # Config file for VS Code
├── 📁 .zed (optional)        # Configurations dir for Zed
│   └── 📄 settings.json      # Config file for Zed
├── 📁 main                   # Directory with the project code
│   ├── 📄 CMakeLists.txt     # CMake file including the main.c file in the project
│   └── 📄 main.c             # File with the app_main entrypoint
├── 📄 .clangd                # Configuration for the clangd language server
├── 📄 .copier_answers.yml    # Answers are recorded here
├── 📄 .gitignore             # Files to ignore in git
├── 📄 CMakeLists.txt         # CMake file configuring the ESP-IDF project
└── 📄 LICENSE (optional)     # LICENSE file, if any
```

## Getting Started

### 1. Install the ESP-IDF framework

Follow the instructions to use the [VS Code extension](https://github.com/espressif/vscode-esp-idf-extension/blob/master/README.md), or install manually in [Windows](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/windows-setup.html) or [Linux/macOS](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/linux-macos-setup.html).

### 2. Install Copier

There are several ways to install copier. It is recommended to install it as a standalone program, either using `pipx`

```bash
pipx install copier
```

or `uv`.

```bash
uv tool install copier
```

### 3. Create the Project

Go to the directory in which you want to create the project, and run

```bash
copier copy --trust gh:EstebanMunoz/esp-idf-template .
```
### 4. Configure IDF paths (Optional)

In case you want an initial build of the generated project, you will need to define the `ìdf_path` and `idf_tools_path` during the questionnaire.
