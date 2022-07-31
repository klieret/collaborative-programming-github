---
theme: default
---

# **Collaborative Programming**

[Kilian Lieret](https://github.com/klieret)

Princeton University

CoDaS-HEP school 2022

Markdown-based slides available as [<mdi-github/> open source](https://github.com/klieret/collaborative-programming-github); contributions welcome!

**Please open these slides on your laptop as we'll jump back and forth between the slides and the browser!**

---

# Structure of this lecture

1. <mdi-github class="text-blue-400"/> **Exploring github in the browser**
  
   1. Creating issues
   2. Forking a repository
   3. Creating commits
   4. Opening pull requests
   5. Handling merge conflicts

2. **Working with a local repository**

3. **Advanced tips & tricks**

---
layout: two-cols
---

# Let's open an issue!



1. Please navigate to [https://github.com/klieret/codas-hep-22-git-playground](https://github.com/klieret/codas-hep-22-git-playground).
2. Open an issue with a random feature request

::right::

**<mdi-checkbox-marked-circle-plus-outline class="text-orange-400"/> Bonus tasks**
   
* Edit the text & title of your issue
* Add a comment mentioning another participant
* Use an emoji reaction
* Close & reopen your issue
* Check for other issues and comment there

**<mdi-crown class="text-red-400"/> Advanced**

* Install the [gh command line tool](https://cli.github.com/)
* Clone the repository
* Use the CL to open an issue

---
layout: two-cols
---


# Forking & committing changes

While you can open issues, you do not have permissions to directly modify content.

1. Click the **fork** button. This will create a "copy" of the whole repository
2. Open the `content` folder and click `Add file` > `Create new file`
3. Call your file `<your gh username>_first` and add a few lines to it

::right::

5. Add a commit message and commit
6. Confirm that you see your file & a new commit

<mdi-alert class="text-red-400"/> Usually you always want to commit to a separate branch in this scenario (later!)

**<mdi-checkbox-marked-circle-plus-outline class="text-orange-400"/> Bonus tasks**
   
1. Add a second file
2. Open your previous file and make changes to the text

**<mdi-crown class="text-red-400"/> Advanced**

Do the same with the gh CLI.

---

# What did we do?

<img src="/feature.svg"/>

* Every node is a commit. Every commit points to a parent. 
* Your fork "branched off" of the original repository: You're adding additional commits to a parallel reality
* Next step: Bringing your commits back to the original repository
* <mdi-alert class="text-blu-400"/> We're being a bit unprecise with the terminology and the picture here; more details later

---

# Creating a PR

* We want to bring our changes back to the original repository
* If you create new commit on a fork, github will already offer you a button to open the PR

**<mdi-checkbox-marked-circle-plus-outline class="text-orange-400"/> Bonus tasks**

* Mention one of your issues. If you write `Closes #<number of your issue>` and the PR is merged, the issue will automatically close.
* Check the differences that the PR will create
* Comment under one of othe differences
* Mention another participant `@<name>`

---

# Branches

<img src="/feature.svg"/>

* If we want to start another PR, we do not need to fork again, we can create another **branch**.
* **Use cases**:
  * Working on several independent experimental features
  * Not all of your PRs might be merged!
* **Branches are cheap** and flexible, go use them!

---

# Forks vs Branches

* A *fork* copies the entire repository:
  * Similar to copying the entire local project folder (including your `.git` repository)
  * If the original repository is deleted, your fork persists
  * You *own* your fork and have every permission there
* A *branch* belongs to its repository and only tracks certain changes
* Branches are cheap and easy, forks are expensive
  * **If you have write permissions for a repository you do not usually need/want to fork it**
    * If you need to fork, fork once and then use branches

---
layout: two-cols
---

# Branches

1. Add another file `content/<your gh username>_second`
2. Select `Create a new branch for this commit and start a pull request`
3. Give your branch a reasonable name (whitespace discouraged)
4. Commit!
5. Create another PR to either:
   * The original repository (`klieret/codas...`)
   * Your own `main` branch (will affect already open PR from this branch)
   * Your neighbors `main` branch (will affect already open PR from this branch)
6. If you receive a PR, merge it

::right::

**<mdi-checkbox-marked-circle-plus-outline class="text-orange-400"/> Bonus tasks**

5. Go back to the default view of your repository and verify that you now have multiple branches
6. Select your new branch
7. Modify your just created file and create a new commit on the same branch
8. Check that your PR has been updated by this new commit

---
layout: two-cols
---

# Merge conflicts

<img src="/merge_conflict.drawio.svg" style="max-height: 50%"/>

::right::

Let's create merge conflicts together!

1. Go to your fork
3. Change something in `content/random-text.txt` (at a random (!) line) and commit it to the branch `merge-conflict`
4. Open a pull request to `klieret/codas...` (`main` branch)

Once some of the PRs are merged, others will show conflicts.

---

# 
