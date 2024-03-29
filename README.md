# Wush - web-push

**wush** - Create and upload a new GitHub repository for a session demo.

## Synopsis

```
wush _[cohort_id]_ _[session]_
```

# Examples

Without any arguments:

```bash
wush
```

With cohort_id argument:

```bash
wush hh-test-24-1
```

With cohort_id and session arguments:

```bash
wush hh-test-24-1 shell-basics
```

## Description

The **wush** script is a tool for creating and uploading a new GitHub repository for a cohort session. It prompts the user for necessary information, such as cohort ID and session name, and performs the required actions to initialize a Git repository and upload it to GitHub.

## Arguments

- **cohort_id**: The unique identifier for the cohort. If not provided as a command-line argument, the script will prompt the user to enter it interactively.

- **session**: The name of the session. If not provided as a command-line argument, the script will prompt the user to enter it interactively.

## Features

### Interactive Mode

If the script is not provided with the required command-line arguments, it enters interactive mode and prompts the user for necessary information.

### Check for Git Repository

The script checks if the current folder is a Git repository. If not, it asks the user for permission to initialize a new one.

### Create and Upload Git Repository

The script then constructs a repository name using the cohort ID and session name. It prompts the user to confirm the creation of a new remote repository on GitHub. If confirmed, the script adds and commits all files to the Git repository and uses the GitHub CLI (`gh`) to create the repository on GitHub, pushing the initial commit.

## See also

- [GitHub CLI (`gh`) documentation](https://cli.github.com/manual/)

## Author

This script was created by Felix Kirchhoff (@F-Kirchhoff).

## Reporting Bugs

Report any issues or bugs on this GitHub repository.
