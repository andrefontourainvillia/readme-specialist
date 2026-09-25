# README Specialist

A GitHub Copilot chat plugin for creating and maintaining clear, practical README documentation while preserving a project's existing tone and style.

[![Install Chat Plugin on VS Code](https://img.shields.io/badge/Install_Chat_Plugin-VS_Code-007ACC)](vscode://chat-plugin/install?source=andrefontourainvillia/readme-specialist)
[![Install Chat Plugin on VS Code Insiders](https://img.shields.io/badge/Install_Chat_Plugin-VS_Code_Insiders-24BFA5)](vscode-insiders://chat-plugin/install?source=andrefontourainvillia/readme-specialist)

## Capabilities

- Creates and restructures README files using established documentation practices.
- Adds practical installation, usage, contributing, and license sections when applicable.
- Writes examples that are easy to follow.
- Keeps documentation consistent with the project's voice and conventions.
- Restricts changes to README and other documentation files.

## Installation

Select the badge for your VS Code edition, then confirm the installation prompt in the editor.

## Usage

1. Open a project in VS Code.
2. Open GitHub Copilot Chat and select the `readme-specialist` agent.
3. Describe the documentation change you need.

Example requests:

```text
Create a README for this project with installation and usage instructions.
```

```text
Update the README to document the new configuration options.
```

```text
Review the README for missing setup steps and outdated examples.
```

## Repository Structure

```text
.
├── agents/
│   └── readme-specialist.agent.md
├── plugin.json
└── README.md
```

- `plugin.json` defines the plugin metadata.
- `agents/` contains the portable agent definition.
- `com.github.copilot/agents/` contains the GitHub Copilot agent definition. (symlink to `agents/`)
- `.plugin/plugin.json` contains plugin-specific configuration and data. (symlink to `plugin.json`)
- `README.md` is the main documentation file for the project.