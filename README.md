# Git commands I use regularly

## Table of Contents

- [Global Options](#global-options)
- [Logs](#logs)
- [Commits](#commits)
- [Inits](#inits)
- [Status](#status)
- [Push and Branches](#push-and-branches)

## Global Options

| Alias | Description                                              | Usage           | Equivalent Command                |
|-------|---------------------------------------------------------|-----------------|-----------------------------------|
| gl    | Displays the contents of the global config file          | `git gl`        | `git config --global -l`          |
| gle   | Opens the global config file in the default editor       | `git gle`       | `git config --global --edit`      |

## Logs

The log has been refurbished to be much more pleasant to look at. The structure is as follows:

$\color{yellow}{\textsf{hash}}$
$\color{red}{\textsf{[}}$
$\color{green}{\textsf{Author date ..}}$
$\color{teal}{\textsf{Author name}}$
$\color{red}{\textsf{]}}$
Commit message

| Alias | Description                                 | Usage         | Equivalent Command           |
|-------|---------------------------------------------|---------------|------------------------------|
| ls    | Log with the last 5 commits                 | `git ls 5`    | `git log -5 HEAD`            |
| lsn   | Log with the last 5 commits and the stats   | `git lsn 5`   | `git log -5 HEAD --stat`     |

## Commits

| Alias | Description                                         | Usage Example                                               | Equivalent Command                                             |
|-------|-----------------------------------------------------|-------------------------------------------------------------|---------------------------------------------------------------|
| ac [files] [message]   | Adds files and commits with message                 | `git ac . "Adding all"`<br>`git ac file1/ file2/ "Updates"` | `git add . && git commit -m "Adding all"`<br>`git add file1/ file2/ && git commit -m "Updates"` |
| ict   | Adds all files and commits with "Initial commit"    | `git ict`                                                   | `git add . && git commit -m "Initial commit"`                 |

## Inits

| Alias | Description                                                                 | Usage    | Equivalent Command                                                                 |
|-------|-----------------------------------------------------------------------------|----------|------------------------------------------------------------------------------------|
| gi    | Creates a new git repo, renames branch, creates .gitignore and README.md    | `git gi` | `git init`<br>`git branch -m master main`<br>`touch .gitignore`<br>`touch README.md`|

## Status

| Alias | Description           | Usage   |
|-------|-----------------------|---------|
| s     | Displays status log   | `git s` |

## Push and Branches

| Alias  | Description                                         | Usage      |
|--------|-----------------------------------------------------|------------|
| gmain  | Switches to main branch                             | `git gmain`|
| eow    | Go to main branch, merge with wip, and pushes       | `git eow`  |