# Contributing

### Set up the environment

```bash
$ virtualenv pelican-blog-venv
$ source pelican-blog-venv/bin/activate
$ pip install pelican markdown
```
### Fork the original repo

[UPLB Eliens Site Repo](https://github.com/uplb-eliens/uplb-eliens.github.io)

This is accomplished in github and you must be logged in. You should have the repository under your account after the fork.

### Clone your fork of the repo

```
$ git clone https://github.com/<YOUR_USERNAME>/uplb-eliens.github.io.git
```

### Configure remote for your forked repo

```
$ git remote -v
$ git remote add upstream https://github.com/uplb-eliens/uplb-eliens.github.io.git
$ git remote -v

```

[Help: Create a remote](https://help.github.com/en/articles/configuring-a-remote-for-a-fork)

### Sync your forked repo with the upstream

```
$ git fetch upstream
$ git checkout master
$ git merge upstream/master
```

[Help: Sync from upstream](https://help.github.com/en/articles/syncing-a-fork)

### Create your blog entry

### Commit and push

### Submit a pull request
