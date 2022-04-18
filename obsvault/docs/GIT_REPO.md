# GIT_REPO

The git repo for this ~~project~~ ~~resume~~ CV (?) is available at two locations.

### Repo Hosts
#### Bitbucket
[Bitbucket](https://bitbucket.org/gsteve3/greg-stevens-career-cv/src/main/)

#### GitHub
[GitHub](https://github.com/gsteve3/greg-stevens-career-cv).


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
    url = git@bitbucket.org:gsteve3/greg-stevens-career-cv.git
    fetch = +refs/heads/*:refs/remotes/origin/*
[branch "main"]
    remote = origin
    merge = refs/heads/main
[remote "gh"]
    url = https://github.com/gsteve3/greg-stevens-career-cv.git
    fetch = +refs/heads/*:refs/remotes/gh/*
[remote "all"]
    url = git@bitbucket.org:gsteve3/greg-stevens-career-cv.git
    fetch = +refs/heads/*:refs/remotes/all/*
    pushurl = git@bitbucket.org:gsteve3/greg-stevens-career-cv.git
    pushurl = https://github.com/gsteve3/greg-stevens-career-cv

```


That extra `[remote "all"]` is the magic to let the below command work:

```shell
git push all
```

Then have both Bitbucket and GittHub's origins updated.

- [ ] #todo #maybe Setup Repo on [[GitLab]].

