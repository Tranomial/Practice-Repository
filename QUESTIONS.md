# Reflection Questions

Answer these as you go — don't wait until the end. Some answers only exist
*after* you've done a step, so fill this in progressively.

Your answers will be reviewed alongside your code. Generic or copy-pasted
answers (that don't reference your actual output) will be sent back for
revision.

---

## Part 1 — Before touching anything (after reading CONTRIBUTING.md)

**1. What branch naming convention does this project use? Give an example
branch name you plan to use.**

> <type>/<short-description>
> docs/hi-my-name-is
> docs because it is a change in the documentation. hi-my-name-is describes what happens in this branch (the hi-my-name-is thing is also a joke but not everyone will get it)

**2. What commit message format is required? Write the exact commit message
you plan to use for your change.**

> <type>: <short-summary>
> docs: Added Ali Ahmed in contributors.md
> docs: resolved merge conflict by adding both Ali Ahmed and Mohamed Nasser as contributors in CONTRIBUTING.md

**3. Does this project expect a linked issue before opening a PR, or is a PR
description enough?**

> Yes, this project expects a linked issue because it resolves issue #1

---

## Part 2 — After forking and cloning

**4. Paste the output of `git remote -v` from your local clone. Which remote
is `origin` and which is `upstream`, and why does that distinction matter?**

> origin  git@github.com:Tranomial/Practice-Repository.git (fetch)
> origin  git@github.com:Tranomial/Practice-Repository.git (push)
> upstream        git@github.com:IbrahimYasserM/Practice-Repository.git (fetch)
> upstream        git@github.com:IbrahimYasserM/Practice-Repository.git (push)
> origin is the fork that only I have full access to
> upstream is the original repo that only the maintainers have access to
> and yes I use SSH :)

---

## Part 3 — After making your change

**5. Paste the output of `git log --oneline -3`. Do your commit message(s)
follow the convention from `CONTRIBUTING.md`?**

> b4e6e5f docs: Added Ali Ahmed in contributors.md
> 3b30f00 (upstream/main, upstream/HEAD, origin/main, origin/HEAD, main) Clarify task labeling in README
> f5ecf54 Revise task assignment instructions in README
> yes, my commit follows the convention


---

## Part 4 — After hitting the seeded merge conflict

**6. What caused the conflict? Which file and lines were involved?**

> Someone added Mohamed Nasser in the line where my name was supposed to go, which is the final line in CONTRIBUTORS.md

**7. How did you resolve it — what did you keep, remove, or combine, and why?**

> I combined both changes, keeping my name and Nasser's name

---

## Part 5 — After opening your PR

**8. Paste your PR link. How many commits and how many files changed does
your PR show?**

> https://github.com/IbrahimYasserM/Practice-Repository/pull/3
> 4 commits, changed one file and added one
> One more commit will be added for this QUESTIONS.md file

---

## Part 6 — Final reflection

**9. What's one thing about this workflow that surprised you, confused you,
or felt different from what you expected going in?**

> Why make an upstream remote? I thought that if I wanted to merge or handle anything from upstream I should fork, clone and work on it local, like for example why did we merge upstream/conflict-practice? Why didn't we fork that branch, clone it and merge the new local conflict-practice?

**10. If a teammate asked you to explain the difference between `fork`,
`clone`, `origin`, and `upstream` in one or two sentences each, what would
you say?**

> Fork is making a copy of a remote repo. The copy is still remote which means it is still on the git server only but you own it and have full access to it.
> Clone is copying a remote repo to your computer which makes it local. You always have full access to local repos.
> Origin is the remote copy of a repo you forked. It is what I was referring to earlier in the "fork" explanation, when I said "The copy is still remote which means..."
> It is the remote repo that is usually available for public in OSS. Sometimes you don't have write access to that repo so you fork it and work on the fork.
