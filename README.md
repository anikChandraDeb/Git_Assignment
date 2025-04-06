# Git_Assignment
🔁 1. --soft Reset

    Command:

git reset --soft <commit>

Effect:

    Moves the HEAD to the specified commit.

    Keeps all your changes staged (in the index).

    Does not touch your working directory.

Use Case:

    When you want to re-commit with a new message or squash commits.

Example:

    git reset --soft HEAD~1
    # The last commit is undone, but the code is still staged.

🔄 2. --mixed Reset (default)

    Command:

git reset --mixed <commit>

Effect:

    Moves HEAD to the specified commit.

    Unstages your changes (clears the index).

    Working directory changes are kept.

Use Case:

    To unstage files but keep your code edits.

Example:

    git reset --mixed HEAD~1
    # The last commit is undone, changes remain in the working directory, but are unstaged.

🔥 3. --hard Reset

    Command:

git reset --hard <commit>

Effect:

    Moves HEAD to the specified commit.

    Clears both the staging area and working directory.

    All changes are lost (cannot be recovered unless backed up).

Use Case:

    To discard all changes and revert to a clean state.

Example:

git reset --hard HEAD~1
# The last commit and any uncommitted changes are permanently deleted.