# Project Overview

This project defines a standardized development environment using VS Code Dev Containers. It is primarily set up for Node.js development, leveraging Node.js version 24. The environment includes a suite of essential development tools, version control enhancements, and shell customizations to provide a consistent and productive coding experience. A key component of this setup is the global installation of `@google/gemini-cli`, indicating its central role in the development workflow within this container.

# Building and Running

This project is designed to be used with [VS Code Dev Containers](https://code.visualstudio.com/docs/devcontainers/containers).

## Building the Development Container

The Docker image for the development environment is defined by the `Dockerfile` located in the `.devcontainer` directory. VS Code will automatically build this image when you first open the project in a Dev Container.

## Running the Development Environment

To use this development environment:

1.  Ensure you have Docker and VS Code with the "Dev Containers" extension installed.
2.  Open this project folder in VS Code.
3.  VS Code will prompt you to "Reopen in Container". Accept this prompt to build and launch the development environment.

Once the container is running, you will have access to all the configured tools and dependencies.

# Development Conventions

## Tools and Extensions

The `.devcontainer/devcontainer.json` file specifies the following VS Code extensions and settings:

*   **Extensions:**
    *   ESLint (`dbaeumer.vscode-eslint`): For code linting.
    *   Prettier (`esbenp.prettier-vscode`): For code formatting.
    *   GitLens (`eamodio.gitlens`): For Git capabilities within the editor.
*   **Formatter:** Prettier is set as the default formatter, with `editor.formatOnSave` enabled.
*   **Linting:** ESLint fixes are applied on save (`editor.codeActionsOnSave` for `source.fixAll.eslint`).

## Shell Configuration

*   **Default Shell:** `zsh` is configured as the default shell.
*   **Plugins:** Includes `git` and `fzf` plugins.
*   **Theme:** `powerlevel10k` theme is used for `zsh`.

## Node.js Environment

*   **Node.js Version:** Node.js 24.
*   **Global Packages:** `@google/gemini-cli` is installed globally, making it available throughout the development environment.
*   **Node Options:** `NODE_OPTIONS` is set to `--max-old-space-size=4096`.