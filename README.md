# Let-s-Learn-Git
Learning git

#Git Commands

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java
$ git config --global user.name
Bhaskar Jaiswal

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java
$ git config --global user.email
bhaskar.jaiswal126@gmail.com

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java
$ ls

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java
$ git init
Initialized empty Git repository in D:/Java/.git/

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ ls

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ ls -a
./  ../  .git/

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Sum.java

nothing added to commit but untracked files present (use "git add" to track)

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git add Sum.java

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Sum.java


Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git commit -m "initial commit"
[master (root-commit) 1d037c1] initial commit
 1 file changed, 8 insertions(+)
 create mode 100644 Sum.java

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git log
commit 1d037c17d9e9988f0ffde57c05c6cc55a1801602 (HEAD -> master)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:35:22 2022 +0530

    initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Sum.java

no changes added to commit (use "git add" and/or "git commit -a")

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git add Diff.java

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Diff.java

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Sum.java


Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git commit -m "Adding Diff.java"
[master 74fd055] Adding Diff.java
 1 file changed, 9 insertions(+)
 create mode 100644 Diff.java

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Sum.java

no changes added to commit (use "git add" and/or "git commit -a")

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git log
commit 74fd05516a070229a4271e900075a55b2581d0af (HEAD -> master)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:43:17 2022 +0530

    Adding Diff.java

commit 1d037c17d9e9988f0ffde57c05c6cc55a1801602
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:35:22 2022 +0530

    initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git add .

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   Sum.java


Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git commit -m "Add modified Sum.java"
[master d07f966] Add modified Sum.java
 1 file changed, 1 insertion(+), 1 deletion(-)

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
nothing to commit, working tree clean

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git log
commit d07f966f8b258846e6fa1dbe7e4ec8d807f4b69c (HEAD -> master)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:46:03 2022 +0530

    Add modified Sum.java

commit 74fd05516a070229a4271e900075a55b2581d0af
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:43:17 2022 +0530

    Adding Diff.java

commit 1d037c17d9e9988f0ffde57c05c6cc55a1801602
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:35:22 2022 +0530

    initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ ^C

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git checkout 1d037c17d9e9988f0ffde57c05c6cc55a1801602
Note: switching to '1d037c17d9e9988f0ffde57c05c6cc55a1801602'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 1d037c1 initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java ((1d037c1...))
$ git status
HEAD detached at 1d037c1
nothing to commit, working tree clean

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java ((1d037c1...))
$ git checkout master
Previous HEAD position was 1d037c1 initial commit
Switched to branch 'master'

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git checkout 1d037c17d9e9988f0ffde57c05c6cc55a1801602
Note: switching to '1d037c17d9e9988f0ffde57c05c6cc55a1801602'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 1d037c1 initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java ((1d037c1...))
$ git branch
* (HEAD detached at 1d037c1)
  master

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java ((1d037c1...))
$ git log
commit 1d037c17d9e9988f0ffde57c05c6cc55a1801602 (HEAD)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:35:22 2022 +0530

    initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java ((1d037c1...))
$ git checkout master
Previous HEAD position was 1d037c1 initial commit
Switched to branch 'master'

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git log
commit d07f966f8b258846e6fa1dbe7e4ec8d807f4b69c (HEAD -> master)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:46:03 2022 +0530

    Add modified Sum.java

commit 74fd05516a070229a4271e900075a55b2581d0af
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:43:17 2022 +0530

    Adding Diff.java

commit 1d037c17d9e9988f0ffde57c05c6cc55a1801602
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:35:22 2022 +0530

    initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ ^C

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git branch dev

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git branch
  dev
* master

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git checkout dev
Switched to branch 'dev'

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (dev)
$ git checkout -b bhaskar/multiply
Switched to a new branch 'bhaskar/multiply'

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (bhaskar/multiply)
$ git status
On branch bhaskar/multiply
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Mul.java

nothing added to commit but untracked files present (use "git add" to track)

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (bhaskar/multiply)
$ git add Mul.java

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (bhaskar/multiply)
$ git status
On branch bhaskar/multiply
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Mul.java


Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (bhaskar/multiply)
$ git commit -m "added Mul.java"
[bhaskar/multiply 9f71fe5] added Mul.java
 1 file changed, 7 insertions(+)
 create mode 100644 Mul.java

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (bhaskar/multiply)
$ git status
On branch bhaskar/multiply
nothing to commit, working tree clean

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (bhaskar/multiply)
$ git log
commit 9f71fe510dfe860b9dc2ccab1fea921b70a59ba6 (HEAD -> bhaskar/multiply)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 18:25:41 2022 +0530

    added Mul.java

commit d07f966f8b258846e6fa1dbe7e4ec8d807f4b69c (master, dev)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:46:03 2022 +0530

    Add modified Sum.java

commit 74fd05516a070229a4271e900075a55b2581d0af
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:43:17 2022 +0530

    Adding Diff.java

commit 1d037c17d9e9988f0ffde57c05c6cc55a1801602
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:35:22 2022 +0530

    initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (bhaskar/multiply)
$ git checkout dev
Switched to branch 'dev'

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (dev)
$ git merge bhaskar/multiply
Updating d07f966..9f71fe5
Fast-forward
 Mul.java | 7 +++++++
 1 file changed, 7 insertions(+)
 create mode 100644 Mul.java

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (dev)
$ git log
commit 9f71fe510dfe860b9dc2ccab1fea921b70a59ba6 (HEAD -> dev, bhaskar/multiply)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 18:25:41 2022 +0530

    added Mul.java

commit d07f966f8b258846e6fa1dbe7e4ec8d807f4b69c (master)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:46:03 2022 +0530

    Add modified Sum.java

commit 74fd05516a070229a4271e900075a55b2581d0af
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:43:17 2022 +0530

    Adding Diff.java

commit 1d037c17d9e9988f0ffde57c05c6cc55a1801602
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:35:22 2022 +0530

    initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (dev)
$ git checkout master
Switched to branch 'master'

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git log
commit d07f966f8b258846e6fa1dbe7e4ec8d807f4b69c (HEAD -> master)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:46:03 2022 +0530

    Add modified Sum.java

commit 74fd05516a070229a4271e900075a55b2581d0af
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:43:17 2022 +0530

    Adding Diff.java

commit 1d037c17d9e9988f0ffde57c05c6cc55a1801602
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:35:22 2022 +0530

    initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git merge dev
Updating d07f966..9f71fe5
Fast-forward
 Mul.java | 7 +++++++
 1 file changed, 7 insertions(+)
 create mode 100644 Mul.java

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git log
commit 9f71fe510dfe860b9dc2ccab1fea921b70a59ba6 (HEAD -> master, dev, bhaskar/multiply)
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 18:25:41 2022 +0530

    added Mul.java

commit d07f966f8b258846e6fa1dbe7e4ec8d807f4b69c
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:46:03 2022 +0530

    Add modified Sum.java

commit 74fd05516a070229a4271e900075a55b2581d0af
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:43:17 2022 +0530

    Adding Diff.java

commit 1d037c17d9e9988f0ffde57c05c6cc55a1801602
Author: Bhaskar Jaiswal <bhaskar.jaiswal126@gmail.com>
Date:   Sun Feb 20 17:35:22 2022 +0530

    initial commit

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ touch .gitignore

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        secretkey.txt

nothing added to commit but untracked files present (use "git add" to track)

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
nothing to commit, working tree clean

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git remote -v

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git remote add origin https://github.com/Bhaskar-ind/Let-s-Learn-Git.git

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git remote -v
origin  https://github.com/Bhaskar-ind/Let-s-Learn-Git.git (fetch)
origin  https://github.com/Bhaskar-ind/Let-s-Learn-Git.git (push)

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git branch -M master

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git push -u origin master
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 8 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (12/12), 1.32 KiB | 450.00 KiB/s, done.
Total 12 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/Bhaskar-ind/Let-s-Learn-Git/pull/new/master
remote:
To https://github.com/Bhaskar-ind/Let-s-Learn-Git.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Diff.java

no changes added to commit (use "git add" and/or "git commit -a")

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git add Diff.ava
fatal: pathspec 'Diff.ava' did not match any files

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git push
Everything up-to-date

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Diff.java

no changes added to commit (use "git add" and/or "git commit -a")

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git add Diff.java

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   Diff.java


Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git push
Everything up-to-date

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git commit -m "added changes in Diff.java"
[master 77ab08f] added changes in Diff.java
 1 file changed, 1 insertion(+), 1 deletion(-)

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 351 bytes | 351.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Bhaskar-ind/Let-s-Learn-Git.git
   9f71fe5..77ab08f  master -> master

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (master)
$ git checkout dev
Switched to branch 'dev'

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (dev)
$ git push -u origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Bhaskar-ind/Let-s-Learn-Git/pull/new/dev
remote:
To https://github.com/Bhaskar-ind/Let-s-Learn-Git.git
 * [new branch]      dev -> dev
Branch 'dev' set up to track remote branch 'dev' from 'origin'.

Ajay Jaiswal@LAPTOP-8EIVF39V MINGW64 /d/Java (dev)
$

