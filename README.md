# Most useful Git Commands

## Content

- [Initiate a repository](#initiate-a-repository)
- [Create a branch](#create-a-branch)

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
