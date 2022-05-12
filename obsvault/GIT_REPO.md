# GIT_REPO

The git repo for this ~~project~~ ~~resume~~ CV (?) is available at two locations.

## Repo Hosts
1. [Bitbucket](https://bitbucket.org/gsteve3/greg-stevens-career/src/main/)
2. [GitHub](https://github.com/gsteve3/greg-stevens-career).
3. [Website](https://career.stevens.pro) powered by [[Obsidian Publish]]


## Tip - Git Push to Multiple Remotes at Once
#ProTip #HowTo


`/.git/config:1`
```properties
[core]
    repositoryformatversion = 0
    filemode = true
    bare = false
    logallrefupdates = true
[remote "origin"]
    url = git@bitbucket.org:gsteve3/greg-stevens-career.git
    fetch = +refs/heads/*:refs/remotes/origin/*
[branch "main"]
    remote = origin
    merge = refs/heads/main
[remote "gh"]
    url = https://github.com/gsteve3/greg-stevens-career.git
    fetch = +refs/heads/*:refs/remotes/gh/*
[remote "all"]
    url = git@bitbucket.org:gsteve3/greg-stevens-career.git
    fetch = +refs/heads/*:refs/remotes/all/*
    pushurl = git@bitbucket.org:gsteve3/greg-stevens-career.git
    pushurl = https://github.com/gsteve3/greg-stevens-career

```


That extra `[remote "all"]` is the magic to let the below command work:

```shell
git push all
```

Then have both Bitbucket and GitHub's origins updated.

### Screenshot `git push all`
*I find this absolutely beautiful.*

![[git push all - WindowsTerminal - benny-win.png]]





---

- [ ] #todo #maybe Setup Repo on [[GitLab]].

