# My Digital Home (directory)

## :heavy_exclamation_mark: WARNING: UNDER CONSTRUCTION :heavy_exclamation_mark:

This is inspired by the work of [Mr. Joshua Corbin Esq.](https://github.com/jcorbin) and his fabulous take on managing one's home.
If you are reading this, I encourage you to checkout [his home](https://github.com/jcorbin/home) on the Githubs.

## Why?

This is the next evolution of my (soon to be) defunct [dotfiles](https://github.com/eculver/dotfiles) repository. It exists to serve a wider purpose of not just managing my dotfiles, but also managing my entire `$HOME`.

The major difference between just "dotfiles" and "home" lies in the reproduceability of my day-to-day environment regardless of which computer I'm actually using.
At the time of creating this repo, I had just gotten a new work laptop and realized how much of a manual process it was to get back to square one where I could start doing work again.

As such, one of the primary goals of this repository is to enable me to go from zero to productive with just a single command (see Installation section below).

## Workflow and Philosophy

Because it's just a git repository, I should mention a few things that make it "unique":

* Everything ignored by default
* Whitelist what git should care about

Similar to [@jcorbin's home](https://github.com/jcorbin/home), I also employ a few other "twists" around git:

* `$HOME`'s only remote is a local repository such as `$HOME/home-int`
* `$HOME` is on a context-specifc, non-master branch (e.g. `personal`, `server`, `debian`, `mac`, etc)
* `$HOME/home-int` has the remotes you'd expect:
** Github for master and other public things
** Private git server for "patron" branches (aka work-related)

## Installation (such meta)

    bash < <(curl -s -S -L https://raw.githubusercontent.com/eculver/home/master/setup.sh)

This executes the following:
- initial fetch of the bootstrap script
- clone this repository
- switches to the appropriate branch for the given environment
- installs all requisite tools and configuration for the environment

After running this, I should be off to the races, committing code at will like a baws.

## Contents

### Applications

Switch to the appropriate architecture branch (i.e. `darwin`, `linux`, etc.) to see what's included

__todo__


### Configuration

__todo__
