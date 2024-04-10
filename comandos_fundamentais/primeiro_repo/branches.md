Here's the translated text with markdown preserved:

## Branching in Git

A branch in Git is a way to separate project versions. When a project is created, it starts in the master branch, but each new feature of the project is kept in a separate branch. It's a good practice for each developer to be responsible for a part of the project to avoid conflicts between branches.

After completing the work on a branch, they are merged to deliver the final source code.

### Creating and Viewing Branches

Creating a branch is commonly used in daily work because when you develop a new feature, a new branch needs to be created.

```bash
git branch first_branch
git branch second_branch
```

When you initialize a branch, it's identical to the master.

### Deleting Branches

```bash
git branch -d second_branch
```

Deleting branches is not common, but it's good practice to maintain the history.

### Switching Branches

Transitioning between branches:

```bash
git checkout master
```

This command switches to the master branch, but be cautious when using it because it carries all changes from the previous branch to the target branch. Save all necessary changes before switching branches.

### Merging Branches

Merging a branch with another developer's branch or with the master:

1. Choose the target branch.

```bash
git checkout master
```

2. Choose the branch you want to merge.

```bash
git merge first_branch
```

3. Resolve conflicts if they exist.

### Stash

Proceeding with another solution but not losing the code you've done so far:

```bash
git stash
```

It goes back to the previous commit but saves the changes made so far.

### Recovering Stash

1. Generate a list of stashes with the saved files.

```bash
git stash list
```

2. After deciding which file to recover, execute:

```bash
git stash <name>
```

### Removing Stash

1. View the list of stashes.

```bash
git stash list
```

2. Remove according to indexing.

```bash
git stash drop 3
```

Note: Removing something is rare to maintain the creation history.

### Creating Tags

The purpose of creating a tag is to have control over the project and understand what's happening with the branch. Tags mark development stages and are widely used in project management.

```bash
git tag -a <name> -m "<msg>"
```

Note: Tagging is not stashing. Tags are usually well-defined to avoid redundancy.

To list tags:

```bash
git tag
```

### Changing Tags

To display details:

```bash
git show <tag>
```

A tag acts as a landmark within the branch. So, by using:

```bash
git checkout <tagName>
```

It's possible to go back to a state before the branch. This is extremely useful. You change the tag according to your project flow. It's a checkpoint within the branch itself.

### Sending Tags to the Repository

You can send these checkpoints to your code and share them among developers.

```bash
git push origin <name>
```

or

```bash
git push origin --tags
```

To send more tags to the project. This is used to change tags according to the version.