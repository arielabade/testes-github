Sure, here are the descriptions of each section along with simple examples, including passing arguments to Git commands where necessary:

## Initial Setup

This section covers the process flow for creating a GitHub repository.

```bash
git init
git add .
git status
git commit -m "Hello world"
git branch -M master
git remote add origin git@github.com:arielabade/testes-github.git
git push -u origin master
```

```bash
git remote rm origin # remove from origin
```

If there's an error with the SSH protocol, try the HTTPS protocol.

## Changes

This section explains the meanings of different statuses in Git:

U = untracked
M = modified

```bash
git status # sets the status
```

## Addition

Describes how to add files to the staging area:

A = added

```bash
git add path/file
git add . \css\styles.css # also adds
git add . 
```

If you don't add a file, it won't be version controlled. So you need to keep adding.

## Commits

Explains how to commit changes:

The goal of commits is to make changes. Specific files or multiple files at once are used with the -a flag.

```bash
git commit a.txt -m "Sending a text"
git commit -m "Sending some texts"
git commit -a -m "Sending ALL texts"
```

Pushing code after committing:

```bash
git push
```

Push is used to sync the master version with other branches. You might see messages like "Your master is behind..." or "Your master is ahead..."

## Receiving Changes

```bash
git pull
```

Used to sync local changes with remote changes. It fetches updates and merges them with the current code (may encounter conflicts). Just pull to update.

## Cloning

```bash
git clone
```

Downloading a remote repository's server. Used when entering a new project.

## Removal

D = deleted

```bash
git rm 
```

Completely removes files and can only be added again with git add. Removal is also an update.

### Change Verification

```bash
git log
```

Accesses the log of modifications made in the project. Provides information about commits made in the projects.

## Rename Files

```bash
 git mv hello.md comandos_fundamentais/hello.md 
 git git mv primeiro_repo/hello.md primeiro_repo/hello.md
```

This is the program's syntax, no need to apply, just know it exists.

## Undo Changes

Used to modify changes to revert to the GitHub state:

```bash
git reset
```

This command resets the file based on everything you've done.

## Git Ignore

Used to ignore files within the project:

```bash
echo hello.md > .gitignore
git add .
git commit -a -m 
```

## Undo Changes

```bash
git reset --hard
```

Undoes all commit changes and dependencies, like doing a hard reset.

