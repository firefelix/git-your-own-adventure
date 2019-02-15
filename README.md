# Welcome to Git Your Own Adventure!

This is a tutorial for advanced git commands on the command line. This tutorial
has a [few requirements](start/requirements.md) that you should check out before you
[start](start/START-HERE.md).

If you are visiting this page for the first time and are still in the original
repo: ie. `onyiny-ang/git-your-own-adventure`, the starting place you are looking for
is [HERE](start/START-HERE.md)

For everyone else,

# Welcome Back to Git Your Own Adventure!

You should now be back in your own github account!! Magic. I know.

You have created a fork of the original which is wholly your own. You can
easily keep it up to date with the original repo, which is useful if, for example, the original is a product
you contribute to and there are a lot of individual contributors working on different aspects of the product. In
that case, you would want to make sure that you're pushing patches or features on
top of the most recent commit to keep the repo up to date and allow your fellow
contributors to easily incorporate your changes.

![Teamwork](https://media.giphy.com/media/yEYiScV53Yeo8/giphy.gif)


On the other hand, a fork can also be useful if you want to keep elements of another developer's work up to a
certain point and diverge after that with your own innovation. This can also be
a perfectly legitimate use of a fork. Fork once and never look back.

![Fork it and forget
it](https://media.giphy.com/media/1ynCulGSsN6f3tRyk0/giphy.gif)


Let's clone the repo into a local directory to continue developing on it.

If you're using https:

```
git clone https://github.com/[my-username]/git-your-own-adventure.git
```

If you've already [set up your ssh key](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/):

```
git clone git@github.com:[my-username]/git-your-own-adventure.git
```

Once you've cloned it locally, we're going to assume, for the purposes of this
tutorial, that you want to collaborate, so you will need to check your remotes.

In the root directory of your clone, in a terminal, type:

```
git remote -v
```

You should see that `origin` is set to your fork. Now we will want to set the
upstream to the original repo. We do this with:

```
git remote add upstream https://github.com/onyiny-ang/git-your-own-adventure.git
```

Now check the remote repositories again

```
git remote -v
```

You should see your fork under `origin` and the original repo under `upstream`.

Before we move on, two more commands you should be familiar with are `fetch` and `merge`.

You can keep your repo up to date with the upstream repo by using `fetch`.

This will fetch all of the recent commits but will not attempt to pull them
into your repo. Depending on what you have done locally since your last
fetch/merge, you may want to do something other than merge. . .we will get to
that later. For now, try fetching the upstream changes and merging them into
your local master branch (Nothing should have
happened yet, so don't expect it to be too exciting this time).

```
git fetch upstream
```

```
git merge upstream/master
```


[Thank you, next](advanced/story-time.md)
