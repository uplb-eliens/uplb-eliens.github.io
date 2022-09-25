# Contributing

### 1. Set up the environment
Tested with Pelican 4.8.0

```bash
$ virtualenv pelican-blog-venv
$ source pelican-blog-venv/bin/activate
$ pip install pelican markdown
```
### 2. Fork the original repo

[UPLB Eliens Site Repo](https://github.com/uplb-eliens/uplb-eliens.github.io)

This is accomplished in github and you must be logged in. You should have the repository under your account after the fork.

### 3. Clone your fork of the repo

```
$ git clone https://github.com/<YOUR_USERNAME>/uplb-eliens.github.io.git
$ cd uplb-eliens.github.io
```

### 4. Configure remote for your forked repo

```
$ git remote -v
$ git remote add upstream https://github.com/uplb-eliens/uplb-eliens.github.io.git
$ git remote -v
```

[Help: Create a remote](https://help.github.com/en/articles/configuring-a-remote-for-a-fork)

### 5. Sync your forked repo with the upstream

```
$ git fetch upstream
$ git checkout master
$ git merge upstream/master
```

[Help: Sync from upstream](https://help.github.com/en/articles/syncing-a-fork)

### 6. Create your blog entry
```
$ mkdir -p content/articles/<YOUR_NICKNAME>
$ mkdir -p content/articles/<YOUR_NICKNAME>/images
```
[Example Article](https://raw.githubusercontent.com/uplb-eliens/uplb-eliens.github.io/master/content/articles/jach/jach_002.rst).

Follow the naming convention above.

If your article has images, place them in the `images` directory.


### 7. Test 

```
$ make clean
$ make html
$ make devserver
```

Check (http://localhost:8000) on browser.

Ctrl+C on the terminal to stop the server when done.


### 7. Commit and push

You might want to sync with upstream first as described above before 
running the following commands.

```
$ git commit -m"edits" -a
$ git push
```

### 8. Exit the environment

```
$ deactivate
```

### 9. Submit a pull request




## Aditional Resources

* [Adding content](https://docs.getpelican.com/en/latest/content.html)
* [RST Syntax](https://github.com/ralsina/rst-cheatsheet/blob/master/rst-cheatsheet.rst) 

