# Obsidian configuration

This repository contains the configuration files which I use in most of my Obsidian vaults.

The content should be put directly to the `.obsidian` subdirectory of the vault directory.

## Community plugins

The community plugins used in the configuration have to be installed manually. Below is the list of their names (versions may be outdated). You have to search for them in the Obsidian settings one by one and install them.

- Auto Link Title
  - Version: 1.5.5 By Matt Furden
- Code Styler
  - Version: 1.1.7 By Mayuran Visakan
- Filename Heading Sync
  - Version: 1.93 By dvcm
- Git
  - Version: 233.0 By Vinzent
- Linter
  - Version: 1.29.0 By Victor Tao
- Open vault in VSCode
  - Version: 1.4.1 By NomarCub
- Quick Links
  - Version: 0.2.5 By Ian Fisher
- Recent Notes
  - Version: 13.1 By Kamil Rudnicki
- Recent Tab Switcher
  - Version: 1.O.1 By Samuel Ang
- Reference Link Render
  - Version: 10.O By njk039

### Plugins just being tested

- Copilot
  - Version: 2.8.9 By Logan Yang
- Smart Connections
  - Version: 25.16 By Brian Petro

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
