---
layout: post
title: "Getting Started with Git"
date: 2013-06-04 07:15
comments: true
categories: 
---

## Getting Git

Head over to the [main git website][git] and download the appropriate git for your OS. Or you could do one of the following:

Linux: `sudo apt-get install git` or `sudo yum install git`

OS X: `brew install git` or just [download the client][git_osx].

Windows: The easiest thing is to use [Chocolatey][chocolatey] and run `cinst git`. Powershell users can also install posh-git: `cinst poshgit`.

## Learning Git

If you wanted to get started with a rapid immersion course on git, I recommend [Git Immersion][gi]. It's a lengthy tutorial, but it's worth it. You'll get a handle on how to work with git as well as guidance on a few of the trickier features.

I know of many intros for the git state of mind. I have a [git setup shell script][gsss] as well as a bunch of links that I've tagged as being git appropriate: [https://pinboard.in/u:peschkaj/t:git](https://pinboard.in/u:peschkaj/t:git)

Los Techies has a multi-part series: [Git for Windows Developers][los].

## Hosting Your Code

* [github](http://github.com) will host open source repositories for free and private repos for a small fee - I think we pay $25 a month for 10 private repositories over at Brent Ozar Unlimited.
* [bitbucket](http://bitbucket.org) will host private repos for free, obviously that's in someone else's control.

You can also self-host git through a variety of mechanisms. 

## Making Git Even Better

On its own, git is a pretty nice version control system. It has some features that can be a bit tricky to work with or remember at first. For that reason, I like to give myself a helping hand on the prompt with a few modifications.

One of the first things I do with any new workstation is install [git-completion][git_c]. Git-completion is a set of auto-complete suggestions for the linux shell. Even if you aren't using bash, there's a git-completion for powershell, too, that you can easily install with [Chocolatey][cinst]. Truthfully, on Windows I'd just install the whole thing via Chocolately. 

[gitflow][gitflow] is essential to maintaining that gittish state of mine. The ideas behind gitflow are explained in [A Successful Git Branching Model][git_branch_success].

Git makes the most sense on the prompt, so Visual Studi/IDE oriented developers may want to start on the command line before moving over to working within the IDE. With [Git integration a native part of Visual Studio 2013][git_vs], it's going to become more important for developers to understand the best ways to work with git and with their dev tools of choice.

## Customizing Git

Git allows for a tremendous amount of customization through the [gitconfig][gitconfig] file in your home directory. Just for a taste, here's what mine looks like:

{% gist https://gist.github.com/peschkaj/5706935 %}

Agile developers may even want to use [git standup][git_standup] to produce a daily summary of activity.

## Further Reading

There's a world of advanced tips out there, like [using `git stash` to hide local changes before pulling down updates][stash_tip].

There's also the [Pro Git book][pro_book] (free) and the [Git screencasts from Peepcode][peep_git] (money).

Other items:

* [Everyday Git](https://www.kernel.org/pub/software/scm/git/docs/everyday.html)
* [Git man page](https://www.kernel.org/pub/software/scm/git/docs/) (for the masochist)
* [Github help](https://help.github.com/)


[git]: http://git-scm.com/
[git_osx]: http://git-scm.com/download/mac
[chocolatey]: http://chocolatey.org/packages?q=git
[gi]: http://gitimmersion.com/
[gsss]: https://gist.github.com/peschkaj/5706191
[los]: http://lostechies.com/jasonmeridth/2009/06/01/git-for-windows-developers-git-series-part-1/
[git_c]: http://git-scm.com/book/en/Git-Basics-Tips-and-Tricks#Auto-Completion
[git_standup]: https://gist.github.com/olim7t/3810376
[cinst]: http://chocolatey.org
[stash_tip]: http://people.planetpostgresql.org/andrew/index.php?/archives/157-Handy-git-tip-number-37.html
[pro_book]: http://git-scm.com/book
[peep_git]: https://peepcode.com/screencasts/git
[gitflow]: https://github.com/nvie/gitflow
[gitconfig]: https://www.kernel.org/pub/software/scm/git/docs/git-config.html
[git_branch_success]: http://nvie.com/posts/a-successful-git-branching-model/
[git_vs]: http://blogs.msdn.com/b/bharry/archive/2013/06/03/visual-studio-2013.aspx