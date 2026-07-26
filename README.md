# AI Flywheel CLI

The command-line interface for installing, managing, validating, and operating the [AI Flywheel Framework](https://github.com/Infoconex/ai-flywheel-framework).

> A loop repeats. A flywheel compounds.

## Purpose

The AI Flywheel CLI provides a consistent way to initialize and manage an AI Flywheel installation inside a software repository.

The CLI is planned as a cross-platform .NET command-line application with support for installation and execution through PowerShell, Bash, and direct .NET tooling.

## Responsibilities

The CLI is responsible for:

- Initializing the AI Flywheel Framework in an existing repository
- Creating and managing missions and goals
- Listing missions and goals with filters
- Updating, pausing, blocking, resuming, and completing work
- Validating framework structure and configuration
- Managing framework upgrades
- Preserving project-specific configuration and knowledge during upgrades
- Providing machine-readable output for automation
- Supporting Windows, Linux, and macOS

## Planned command model

```text
flywheel init
flywheel mission create
flywheel mission list
flywheel goal create
flywheel goal list
flywheel validate
flywheel upgrade
```

The final command surface will evolve through implementation and validation against real Flywheel workflows.

## Relationship to the AI Flywheel ecosystem

| Repository | Responsibility |
|---|---|
| [ai-flywheel-spec](https://github.com/Infoconex/ai-flywheel-spec) | Defines the normative specification |
| [ai-flywheel-framework](https://github.com/Infoconex/ai-flywheel-framework) | Provides the official installable implementation |
| **ai-flywheel-cli** | Installs, manages, validates, and operates the framework |
| [ai-flywheel-sample](https://github.com/Infoconex/ai-flywheel-sample) | Demonstrates the framework and CLI together |

## Technology direction

The initial implementation will target .NET 10 and prioritize:

- A simple cross-platform executable
- Clear and stable commands
- Script-friendly output and exit codes
- PowerShell and Bash installation paths
- Testable separation between command handling and Flywheel operations

## Status

This repository is under active development. The initial focus is onboarding, core mission and goal management, validation, and cross-platform installation.

## License

Licensing information will be added as the project is formalized.
