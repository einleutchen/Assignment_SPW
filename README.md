### Assignment_SPW
This is the project for SPW lecture

# What is Branch?
In Git, a branch is a lightweight, movable pointer to a commit. Instead of copying all files, Git simply tracks where your work diverges from
the main line. It represents an independent line of development. Unlike older version control systems, Git does not copy all your files when
you create a branch. Instead, it simply remembers which commit you are currently working on. This makes branching in Git  fast and "cheap" in
terms of storage. 

- The HEAD Pointer: Git uses a special pointer called HEAD to track the current branch you are working on. When switch branches, HEAD moves
to the new branch pointer.
- Efficient Storage: Git only stores the differences between branches. Identical files are shared, meaning branching costs almost no disk 
space and is nearly instantaneous.

## Purpose: Isolation & Safety
The primary goal of branching is isolation. It allows for:

- Independent Development: Changes made in a branch do not affect the main project until they are intentionally merged.
- Stability: The main line of development (usually called main) remains stable and deployable, while experimental or incomplete code is kept separate.
- Risk Management: If a feature or an experiment fails, the branch can be deleted without any impact on the rest of the project.

## The "Feature Branch" Workflow
This is the industry-standard strategy for working in teams:

- Task-Oriented: A dedicated branch is created for every new task (e.g., a new feature, a bug fix, or a UI update).
- Quality Control:  This ensures that the main branch only contains tested, production-ready code.
- Parallel Work: It facilitates collaboration, as multiple developers can work on different tasks simultaneously without interfering with 
each other.

## Essential Commands for Branch Management
**git branch** Lists all existing branches in the repository
**git branch NAME**  Creates a new branch at the current commit
**git checkout NAME** Switches the working directory to the specified branch
**git checkout -b NAME**  A combined command to create and switch to a new branch immediately
**git push origin NAME** - Uploads the local branch to a remote server (GitHub)


