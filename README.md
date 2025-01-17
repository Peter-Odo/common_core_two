<!-- VERSION CONTROL -->

# WHAT IS VERSION CONTROL

- Version control is a system that allows us (engineers) to track, manage changes to a software code (code base) over time. It helps keep a history of changes, enables collaboration.

## Core Concepts

[x] Snapshots of project

- Every time changes are committed, a snapshot of the current project state is saved
- These snaphots allow engineers (us) to view, compare, or roll back to any previous version.

[x] Collaboration

- Multiple engineers can work on the same codebase at the same time, without overiding each other's changes.
- Branching and merging enable simultaneous work on different features, scripts or bug fixes.

[x] Change Tracking

- Version control records who made what changes, when and why.
- This is essential for debugging and accountability

## Why It's Important

- Enables seamless collaboration in large teams.
- Ensures a reliable history changes, critical for audits or debugging
- Protects against data loss by storing project history in remote repositories

## Benefits of GIT

#### Git, a distributed version control system, stands out because of its features and widespread adoption

[x] Decentralized Nature: Each contributor has a full copy of the repository, including the entire history. Work can continue offline and changes can be synced later.

[x] Performance: Git is optimized for speed, enabling quick branching, merging and history lookups.

[x] Collaboration: Features like branches, pull requests and merge options.

[x] Support Automation: Integrates seamlessly with CI/CD pipelines, cloud environments and DevOps tools

## Git Basics

[x] Setting up GIT: Before using git, we need to install and configure it on our machines

- Linux:

```
sudo apt-get install git
```

- Mac:

```
brew install git
```

- Windows:

```
https://git-scm.com
```

[x] To verify if git is installed properly:

```
git --version
```

## Core commands

[x] Initialize a repository (folder): This creates a `.git` folder in our project directory, enabling Git tracking.

```
git init
```

[x] Check repository status: Display the state of the working directory and staging area. Shows untracked files and changes yet to be committed.

```
git status
```

[x] Stage changes: Staging allows us to select specific changes for the next commit

```
git add <file_name>    # Stage a specific file
git add .              # Stage all changes
```

[x] Commit changes: Commits take a snapshot of the staged changes.

```
git commit -m 'Describe your changes'
```

[x] Push changes: Uploads local commits to a remote repository (e.g., GitHub)

```
git push origin <branch_name>
```

## Collaborating with Branches

### What is a branch?

- A branch is a pointer to specific commit, allowing us to work features or fixes independently of the main (master) code base.
- Main Branch (main, master, production): The default branch (for production-ready code).
- Feature Branches: Temporary branches created for specific tasks (e.g, feature-update-config-files)

[x] Create a branch

```
git branch <branch_name>    # Creates branch

git checkout -b <branch_name> # Creates branch and switches us to that branch
```

[x] Switch to the Branch

```
git checkout <branch_name>
```
