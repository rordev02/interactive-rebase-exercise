# Interactive Rebase Exercise
This repo is to practise the art of [Rewiting Git History](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History). Anyone can practice the interactive reabse with the help of this repository.

### Insight
#### Changing the Last Commit

Changing your most recent commit is probably the most common rewriting of history that you’ll do. You’ll often want to do two basic things to your last commit: simply change the commit message, or change the actual content of the commit by adding, removing and modifying files.
```bash
git commit --amend
```

#### Changing Multiple Commit Messages

To modify a commit that is farther back in your history, you must move to more complex tools. Git doesn’t have a modify-history tool, but you can use the rebase tool to rebase a series of commits onto the HEAD that they were originally based on instead of moving them to another one. With the interactive rebase tool, you can then stop after each commit you want to modify and change the message, add files, or do whatever you wish. You can run rebase interactively by adding the -i option to git rebase. You must indicate how far back you want to rewrite commits by telling the command which commit to rebase onto.
```bash
git rebase -i
```

For example, if you want to change the last three commit messages, or any of the commit messages in that group, you supply as an argument to `git rebase -i` the parent of the last commit you want to edit, which is `HEAD~3`. because you’re trying to edit the last three commits.
```bash
git rebase -i HEAD~3
```

### To-Do

This main branch have mutiple **commit in random order and name**. The task is to **use interactive rebase**  to put commits in [**correct manner**](#correct-manner).

To start the practice perfrom these steps:
- Create a branch with **your name** of you choosing & add **timestamp** in **YYYYMMDDHHMMSS** as **prefix** it. For Exmaple `berlin-20211208164937`
- Then use **interactive rebase**  to put commits in [**correct manner**](#correct-manner).


### Random Commits
-

### Correct Manner

- Exmaple 1
- Exmaple 2
- Exmaple 3
- Exmaple 4

Exmaple 1 must contain all the commits starts with Exmaple 1 only and same for other commits too They should only contain Examples of there respective number.