# Obsidian configuration

This repository contains the configuration files which I use in most of my Obsidian vaults.

The content should be put directly to the `.obsidian` subdirectory of the vault directory.

## Community plugins

The community plugins used in the configuration have to be installed manually. Below is the list of their names (versions may be outdated). You have to search for them in the Obsidian settings one by one and install them.

| Name                   | Version | Author         |
|------------------------|---------|---------------|
| Auto Link Title        | 1.5.5   | Matt Furden   |
| Code Styler            | 1.1.7   | Mayuran Visakan|
| Filename Heading Sync  | 1.93    | dvcm          |
| Git                    | 233.0   | Vinzent       |
| Linter                 | 1.29.0  | Victor Tao    |
| Open vault in VSCode   | 1.4.1   | NomarCub      |
| Quick Links            | 0.2.5   | Ian Fisher    |
| Recent Notes           | 13.1    | Kamil Rudnicki|
| Recent Tab Switcher    | 1.0.1   | Samuel Ang    |
| Reference Link Render  | 10.0    | njk039        |

### Plugins just being tested

| Name              | Version | Author      |
|-------------------|---------|------------|
| Copilot           | 2.8.9   | Logan Yang  |
| Smart Connections | 25.16   | Brian Petro |

## About the repository

If you need a testing branch to be checked out, you can add the `main` branch as a git worktree. Then it is easier to cherry-pick the changes to the main branch. VS Code will show the worktree as another repository in Source Control but you might need to navigate to the `.worktrees/main` directory to initiate the detection.

``` shell
git worktree add .worktrees/main/ main
```

## TODO

- [ ] Add pre-commit hook to check for sensitive data in the configuration files.
- [ ] Describe the goals of the configuration.
- [x] Check the way community plugins should be installed.
  - They are not installed automatically. The user is not notified about the missing plugins.
- [x] Check if the installed plugins will not overwrite their configuration files.
  - The configuration files which existed before the plugin installation seem not to be overwritten.
