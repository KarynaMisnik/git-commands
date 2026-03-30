# Most useful Git Commands

## Content

- [Initiate a repository](#initiate-a-repository)
- [Working in team repo](#working-in-team-repo)
- [Pulling request](#pulling-request)

### Initiate a repository

The flow of working with a new repository:

```bash
git init
// run the command in working directory to initiate a repo
```

Make changes in the repo or its files:

```bash
git add .
//stage all changes
git commit -m "first commit"
// Changes won’t be committed without a message
```

To pconnect to remote Github repo:

```bash
git remote add origin <url>
```

Finally, to push all changes to a repo:

```bash
git push -u origin main
// it will be pushed to main branch
```

To check what is current working branch:

```bash
git branch
```

To rename branch to match remote branch name:

```bash
git branch -M main
```

### Working in team repo

To copy a remote repo:

```bash
git clone <url>
```

Create your working branch (NEVER push changes into main branch without permission):

```bash
git switch -c feature-name
```

OR

```bash
git checkout -b feature-name
// give a descriptive brach name
```

Make changes in a project files, save changes, stage changes:

```bash
git add .
git commit -m "what you did"
// write descriptive but short comments
```

Push changes to remote repo:

```bash
git push -u origin feature-name
```

> Note: Before starting work (good habit)

```bash
git status // see local changes
git pull // make sure you're up to date with remote
```

### Pulling request
