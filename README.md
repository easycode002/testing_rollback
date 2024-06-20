## How to rollback project in Github on specific point of time.

> [!NOTE] 
> For rollback project with specific time, it is absolutely necessary to create a new branch to affect the whole project or other branches.
#### check commit ID
```
git log
```
Example, after run this command it return
`
commit 6822c793866f8aa2bd1d4178c8ff8b01e48e6ffb22
...
...
`

#### Create new branch, and switch to new branch
```
git checkout -b <branch_name>
```

#### Rollback project specific time to new branch
```
git checkout -b rollback-branch 6822c793866f8aa2bd1d4178c8ff8b01e48e6ffb22
```
`
Noted rollback-branch is new branch after create
`

#### Push the new branch to GitHub
```
git push origin rollback-branch
```

`Commit 001`