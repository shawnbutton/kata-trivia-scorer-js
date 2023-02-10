# Trivia Scorer

This is the Trivia Scorer kata in TypeScript

# Kata Instructions

In this kata you will create a program to calculate scores on a trivia quiz.

You will be passed a string indicating which answers the user got right and wrong, and will return a number indicating their score.

The instructions are in the links below. Please finish each before proceeding to the next one.

[trivia_scorer1.md](instructions/trivia_scorer1.md)  
[trivia_scorer2.md](instructions/trivia_scorer2.md)  
[trivia_scorer3.md](instructions/trivia_scorer3.md)  
[trivia_scorer4.md](instructions/trivia_scorer4.md)  
[trivia_scorer5.md](instructions/trivia_scorer5.md)  
[trivia_scorer6.md](instructions/trivia_scorer6.md)  
[trivia_scorer7.md](instructions/trivia_scorer7.md)  
[trivia_scorer8.md](instructions/trivia_scorer8.md)

# Facilitators Notes

This kata is designed to practice Test Driven Development.
The kata requirements are given in sequential files in order to encourage working in small steps.

## Guidance for mob.sh

Mob.sh is a simple GO script that facilitates mobbing and pairing using a git
branch as a go-between. It aims to be very simple in its implementation.

### TL;DR

- `brew install remotemobprogramming/brew/mob`
- `mob start -b [unique_name]` starts a mob session with a uniquely named
  coordination branch
- `mob next` to hand control off to the next pilot
- `mob start -b [unique_name]` to pick-up control for the next pilot
- `mob done` when you're done to drop all changes (squashed, staged) ready to
  commit to the branch you started in

### Setting Up

Ensure you have mob.sh installed:

```
brew install remotemobprogramming/brew/mob
```

### Usage

The person starting off the mob session starts in the master branch of the
repository and types:

```
mob start -b (choose a unique name)
```

_Note: It's important when there may be many simultaneous mob/pairing sessions
within a repository to specify a unique name for your particular mob session.
This determines a unique branch name for coordination that won't clash with
other sessions. The branch name used for the mob session will end up looking
something like `mob/master/story123456`._

For a unique name, choose something that suits you:

- a story number
- a handle
- something random or made up
- no spaces or punctuation!

This places you in a special branch in which all mobbing takes place until your
session is complete.

There is no need to make discreet commits - commits along the mob branch are
squashed and presented at the end as a set of uncommitted files in the branch in
which you started.

When the first pilot is ready to hand the session off to a co-pilot, they issue
the command:

```
mob next
```

This will create a work-in-progress commit, push the changes up to the git repo,
and will then be ready for the next pilot to take control.

The next pilot takes control with:

```
mob start -b (the same unique name you started with)
```

And this is how it goes as you bounce control between the pilots in your mobbing
session. When the session is done, the last pilot issues:

```
mob done
```

This will squash all work-in-progress commits along the mob branch and present
them as uncommited changes to the master. It's then just a normal commit to
master for all the work completed by everyone in the mob.

For example:

```
git commit -am "describe the work done here, tag a jira ticket"
git push
```

And that's it!

Happy Mobbing / Pairing!

Please direct any questions to Pascal Maniraho <pascal.maniraho@rbc.com> or Shawn Button <shawn.button@rbc.com>.
