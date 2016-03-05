#brunch

`brunch` tells you what git branches you're on.

###Setup

```
$ git clone https://github.com/bentarnoff/brunch.git
$ cd brunch
$ bundle install
```

r2u pulls the info about the repos and URIs from the config YAMLs of the book repos. Make sure that `docs-book-cloudfoundry`, `docs-book-pivotalcf`, and `docs-book-runpivotal` are all in your `workspace` directory.

###Usage

Run `brunch` from your `~/workspace` directory.

`brunch -a`

**Lists your current git branch in all directories under your present working directory.**

`brunch -m`

**Lists only those directories where your current git branch is master.**

`brunch -n`

**Lists only those directories where your current git branch is not master.**

`brunch -b YOUR-BRANCH`

**Lists only those directories where your current git branch is YOUR-BRANCH.**


###Add it to your bash_profile

```
$ echo "alias brunch='ruby ~/workspace/brunch/brunch.rb'" >> ~/.bash_profile
```

Now you can run it with:

```
$ brunch
```
