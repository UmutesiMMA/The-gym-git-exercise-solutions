# The-gym-git-exercise-solutions
## Bundle 1
### Exercise 1
```bash
user@DESKTOP-TQVNUUS MINGW64 ~
$ cd ~/Documents/TheGym/Project

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project
$ git init
Initialized empty Git repository in C:/Users/user/Documents/TheGym/Project/.git/

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (master)
$ git branch -m "master" "main"

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch start.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch story.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch notes.txt

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch review.txt

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ ls
lamp.jpeg  review.txt  step.jpeg   trees-lamp.jpeg
notes.txt  start.html  story.html
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git mv review.txt feedback.txt

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   feedback.txt
        new file:   lamp.jpeg
        new file:   notes.txt
        new file:   start.html
        new file:   step.jpeg
        new file:   story.html
        new file:   trees-lamp.jpeg


user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git commit -m "First"
[main (root-commit) d1e51b8] First
 7 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 feedback.txt
 create mode 100644 lamp.jpeg
 create mode 100644 notes.txt
 create mode 100644 start.html
 create mode 100644 step.jpeg
 create mode 100644 story.html
 create mode 100644 trees-lamp.jpeg

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git remote add origin https://github.com/UmutesiMMA/The-gym-git-exercise-solution.git

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git branch -M main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push -u origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 5.00 MiB | 1.07 MiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git switch -c dev
Switched to a new branch 'dev'

 user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (dev)
$ git push origin dev
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 5.00 MiB | 682.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/d
ev
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      dev -> dev

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (dev)
$ git switch -c test
Switched to a new branch 'test'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/t
est
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      test -> test

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (test)
$ git switch dev
Switched to branch 'dev'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (dev)
$ git branch -d test
Deleted branch test (was d1e51b8).

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (dev)
$ git push origin --delete test
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 - [deleted]         test
```

### Exercise 2

```bash
user@DESKTOP-TQVNUUS MINGW64 ~
$ cd ~/Documents/TheGym/Project/

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (dev)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch home.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash
Saved working directory and index state WIP on main: d1e51b8 First

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch about.hhtml

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch about.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add about.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash -m "about page"
Saved working directory and index state On main: about page

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch team.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add team.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash -m "team page"
Saved working directory and index state On main: team page

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (708dd030faf601bbf98cc41067442e5c4df45abf)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash list
stash@{0}: On main: team page
stash@{1}: WIP on main: d1e51b8 First

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (e014cca4c5401550881d92b1cc4a8435d657429f)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git commit -m "Team page not included"
[main 35a55b2] Team page not included
 2 files changed, 32 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git fetch origin
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 9 (delta 5), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (9/9), 3.20 KiB | 25.00 KiB/s, done.
From https://github.com/UmutesiMMA/The-gym-git-exercise-solutions
   d1e51b8..42f1a9b  main       -> origin/main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git pull
Merge made by the 'ort' strategy.
 README.md | 212 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 212 insertions(+)
 create mode 100644 README.md

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 1.04 KiB | 266.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   42f1a9b..d63f8d9  main -> main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$
```
## Bundle 2
### Exercise 1
```bash
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (main)
$ git switch -c ft/bundle-2
Switched to a new branch 'ft/bundle-2'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
$ touch service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
$ git add service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
$ git commit -m "Service page"
[ft/bundle-2 fac79a3] Service page
 1 file changed, 18 insertions(+)
 create mode 100644 service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
$ git push origin ft/bundle-2
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 4 threads
Compressing objects: 100% (18/18), done.
Writing objects: 100% (18/18), 4.53 KiB | 356.00 KiB/s, done.
Total 18 (delta 9), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (9/9), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/f
t/bundle-2
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
$
```

### Exercise 2
```bash

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/service-redesign)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/service-redesign)
$ git commit -m "new changes in service redesign branch"
[ft/service-redesign dff22e4] new changes in service redesign branch
 1 file changed, 20 insertions(+)
 create mode 100644 service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 563 bytes | 187.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/f
t/service-redesign
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/bundle-2)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ ls
README.md   feedback.txt  lamp.jpeg  start.html  story.html
about.html  home.html     notes.txt  step.jpeg   trees-lamp.jpeg

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git pull
remote: Enumerating objects: 13, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 9 (delta 5), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (9/9), 3.26 KiB | 37.00 KiB/s, done.
From https://github.com/UmutesiMMA/The-gym-git-exercise-solutions
   d63f8d9..de9b1d9  main                 -> origin/main
 * [new branch]      revert-3-ft/bundle-2 -> origin/revert-3-ft/bundle-2
Updating d63f8d9..de9b1d9
Fast-forward
 README.md    | 78 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 service.html | 18 ++++++++++++++
 2 files changed, 96 insertions(+)
 create mode 100644 service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ ls
README.md   feedback.txt  lamp.jpeg  service.html  step.jpeg   trees-lamp.jpeg
about.html  home.html     notes.txt  start.html    story.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git commit -m "changes on same line different branches"
[main 3c7d551] changes on same line different branches
 1 file changed, 2 insertions(+), 1 deletion(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 361 bytes | 120.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   de9b1d9..3c7d551  main -> main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/service-redesign)
$ git diff ft/service-redesign main
diff --git a/README.md b/README.md
index c510bc8..34c5cea 100644
--- a/README.md
+++ b/README.md
@@ -207,6 +207,84 @@ $ git commit -m "Team page not included"
  2 files changed, 32 insertions(+)
  create mode 100644 about.html
  create mode 100644 home.html
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
+$ git fetch origin
+remote: Enumerating objects: 10, done.
+remote: Counting objects: 100% (10/10), done.
+remote: Compressing objects: 100% (9/9), done.
+remote: Total 9 (delta 5), reused 0 (delta 0), pack-reused 0
+Unpacking objects: 100% (9/9), 3.20 KiB | 25.00 KiB/s, done.
+From https://github.com/UmutesiMMA/The-gym-git-exercise-solutions
+   d1e51b8..42f1a9b  main       -> origin/main
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
+$ git push origin main
+To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
+ ! [rejected]        main -> main (non-fast-forward)
+error: failed to push some refs to 'https://github.com/UmutesiMMA/The-gym-git-exerc
ise-solutions.git'
+hint: Updates were rejected because the tip of your current branch is behind
+hint: its remote counterpart. Integrate the remote changes (e.g.
+hint: 'git pull ...') before pushing again.
+hint: See the 'Note about fast-forwards' in 'git push --help' for details.
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
+$ git pull
+Merge made by the 'ort' strategy.
+ README.md | 212 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+ 1 file changed, 212 insertions(+)
+ create mode 100644 README.md
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
+$ git push origin main
+Enumerating objects: 8, done.
+Counting objects: 100% (8/8), done.
+Delta compression using up to 4 threads
+Compressing objects: 100% (6/6), done.
+Writing objects: 100% (6/6), 1.04 KiB | 266.00 KiB/s, done.
+Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
+remote: Resolving deltas: 100% (2/2), completed with 1 local object.
+To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
+   42f1a9b..d63f8d9  main -> main

+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
+$
+
```
## Bundle 2
### Exercise 1
```bash
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (main)
+$ git switch -c ft/bundle-2
+Switched to a new branch 'ft/bundle-2'
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
+$ touch service.html
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
+$ git add service.html
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
+$ git commit -m "Service page"
+[ft/bundle-2 fac79a3] Service page
+ 1 file changed, 18 insertions(+)
+ create mode 100644 service.html
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
+$ git push origin ft/bundle-2
+Enumerating objects: 19, done.
+Counting objects: 100% (19/19), done.
+Delta compression using up to 4 threads
+Compressing objects: 100% (18/18), done.
+Writing objects: 100% (18/18), 4.53 KiB | 356.00 KiB/s, done.
+Total 18 (delta 9), reused 0 (delta 0), pack-reused 0
+remote: Resolving deltas: 100% (9/9), completed with 1 local object.
+remote:
+remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
+remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/
f
+t/bundle-2
+remote:
+To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
+ * [new branch]      ft/bundle-2 -> ft/bundle-2

+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
+$
diff --git a/service.html b/service.html
index 89fdab2..59a54fe 100644
--- a/service.html
+++ b/service.html
@@ -8,13 +8,12 @@
 </head>
 <body>

-    <di> Services we provide</di>
+    <di> Services that our company provides include:</di>
     <ul><li>Sell</li>
         <li>Repair</li>
         <li>Make from scratch</li>
+        <li> Buy </li>

     </ul>
-    <div>Coupons:</div>
-    <div>How to access out services</div>
 </body>
 </html>
\ No newline at end of file

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/service-redesign)
$ git merge main
Auto-merging service.html
CONFLICT (add/add): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/service-redesign|MERGING)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/service-redesign|MERGING)
$ git commit -m "Merging main with ft/service-redesign"
[ft/service-redesign bf35848] Merging main with ft/service-redesign

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 233 bytes | 116.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   dff22e4..bf35848  ft/service-redesign -> ft/service-redesign
```
### Bundle3
## Exercise 1
```bash
user@DESKTOP-TQVNUUS MINGW64 ~
$ cd ~/Documents/TheGym/Project

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git switch ft/faq-page
Switched to branch 'ft/faq-page'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git log
commit 6e65ae42442d49061859ff16f03ce4549be522b2 (HEAD -> ft/faq-page, origin/ft/faq-
page)
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 11:06:53 2023 +0300

    Frequently asked questions

commit 97c390cfbb91cef566bb1c03ac6fbfc7d4e5412f (origin/ft/contact-page, ft/contact-
page)
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 10:54:40 2023 +0300

    list of managers in team

commit 1a5d253bb2c895b5d5a2b4441e0078d128b800d7
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 10:26:32 2023 +0300

    team page in ft/team-page branch

commit 3c7d5510c081878f1cd856b2fd9c658983e9bc22
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 00:23:31 2023 +0300

    changes on same line different branches

commit de9b1d9903afb32e519bd524da372bff3fb0dd6a
Merge: 1e2cd02 fac79a3
Author: UmutesiMMA <133501822+UmutesiMMA@users.noreply.github.com>
Date:   Thu May 18 16:19:49 2023 +0300

    Merge pull request #3 from UmutesiMMA/ft/bundle-2

    Service page added

commit 1e2cd025fc40e34fc0c73eaa1cad172f34701111
Author: UmutesiMMA <133501822+UmutesiMMA@users.noreply.github.com>
Date:   Thu May 18 01:29:47 2023 +0300

    B2/E1

commit fac79a3659e3a5c6543c5fc65bd8b4fa134927d6 (origin/ft/bundle-2, ft/bundle-2)
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Thu May 18 01:22:00 2023 +0300

    Service page


user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git revert 1a5d253bb2c895b5d5a2b4441e0078d128b800d7
CONFLICT (modify/delete): team.html deleted in parent of 1a5d253 (team page in ft/te
am-page branch) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert 1a5d253... team page in ft/team-page branch
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page|REVERTING)
$ git revert --continue
error: Committing is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
U       team.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page|REVERTING)
$ git revert --skip

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git commit -m "new changes"
On branch ft/faq-page
nothing to commit, working tree clean

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git push origin ft/faq-page
Everything up-to-date

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git add team.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git commit -m "new team member"
[ft/faq-page 7696850] new team member
 1 file changed, 1 insertion(+)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 320 bytes | 106.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   6e65ae4..7696850  ft/faq-page -> ft/faq-page

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git log
commit 76968504ae363a30e124c7659c20264131474689 (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Tue May 23 20:51:58 2023 +0300

    new team member

commit 6e65ae42442d49061859ff16f03ce4549be522b2
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 11:06:53 2023 +0300

    Frequently asked questions

commit 97c390cfbb91cef566bb1c03ac6fbfc7d4e5412f (origin/ft/contact-page, ft/contact-page)
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 10:54:40 2023 +0300

    list of managers in team

commit 1a5d253bb2c895b5d5a2b4441e0078d128b800d7
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 10:26:32 2023 +0300

    team page in ft/team-page branch

commit 3c7d5510c081878f1cd856b2fd9c658983e9bc22
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 00:23:31 2023 +0300

    changes on same line different branches

commit de9b1d9903afb32e519bd524da372bff3fb0dd6a
Merge: 1e2cd02 fac79a3
Author: UmutesiMMA <133501822+UmutesiMMA@users.noreply.github.com>
Date:   Thu May 18 16:19:49 2023 +0300

    Merge pull request #3 from UmutesiMMA/ft/bundle-2

    Service page added

commit 1e2cd025fc40e34fc0c73eaa1cad172f34701111
Author: UmutesiMMA <133501822+UmutesiMMA@users.noreply.github.com>
Date:   Thu May 18 01:29:47 2023 +0300

    B2/E1

commit fac79a3659e3a5c6543c5fc65bd8b4fa134927d6 (origin/ft/bundle-2, ft/bundle-2)
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git revert 1a5d253bb2c895b5d5a2b4441e0078d128b800d7
CONFLICT (modify/delete): team.html deleted in parent of 1a5d253 (team page in ft/team-page b
ranch) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert 1a5d253... team page in ft/team-page branch
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page|REVERTING)
$ git add team.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page|REVERTING)
$ git revert --continue
On branch ft/faq-page
You are currently reverting commit 1a5d253.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

nothing to commit, working tree clean

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page|REVERTING)
$ git revert --continue
On branch ft/faq-page
You are currently reverting commit 1a5d253.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

nothing to commit, working tree clean

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page|REVERTING)
$ git revert --continue
On branch ft/faq-page
You are currently reverting commit 1a5d253.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

nothing to commit, working tree clean

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page|REVERTING)
$ git revert --skip

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git log
commit 76968504ae363a30e124c7659c20264131474689 (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Tue May 23 20:51:58 2023 +0300

    new team member

commit 6e65ae42442d49061859ff16f03ce4549be522b2
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 11:06:53 2023 +0300

    Frequently asked questions

commit 97c390cfbb91cef566bb1c03ac6fbfc7d4e5412f (origin/ft/contact-page, ft/contact-page)
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 10:54:40 2023 +0300

    list of managers in team

commit 1a5d253bb2c895b5d5a2b4441e0078d128b800d7
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 10:26:32 2023 +0300

    team page in ft/team-page branch

commit 3c7d5510c081878f1cd856b2fd9c658983e9bc22
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 00:23:31 2023 +0300

    changes on same line different branches

commit de9b1d9903afb32e519bd524da372bff3fb0dd6a
Merge: 1e2cd02 fac79a3
Author: UmutesiMMA <133501822+UmutesiMMA@users.noreply.github.com>
Date:   Thu May 18 16:19:49 2023 +0300

    Merge pull request #3 from UmutesiMMA/ft/bundle-2

    Service page added

commit 1e2cd025fc40e34fc0c73eaa1cad172f34701111
Author: UmutesiMMA <133501822+UmutesiMMA@users.noreply.github.com>
Date:   Thu May 18 01:29:47 2023 +0300

    B2/E1

commit fac79a3659e3a5c6543c5fc65bd8b4fa134927d6 (origin/ft/bundle-2, ft/bundle-2)
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
:
```

## Exercise 2
```bash
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git checkout -b ft/home-redesign
Switched to a new branch 'ft/home-redesign'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git commit -m "changes to home page"
[main 7b6219d] changes to home page
 1 file changed, 2 insertions(+), 1 deletion(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 402 bytes | 201.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   1bc787e..7b6219d  main -> main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git switch ft/home-redesign
Switched to branch 'ft/home-redesign'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-redesign.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git add home.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git commit -m "nav bar on home page"
[ft/home-redesign fed2d79] nav bar on home page
 1 file changed, 8 insertions(+)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git push origin ft/home-redesign
Enumerating objects: 14, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 4 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (12/12), 1.45 KiB | 370.00 KiB/s, done.
Total 12 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-redesign' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/f
t/home-redesign
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      ft/home-redesign -> ft/home-redesign

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$
```
### Bundle4
## Exercise 1
```bash

```

## Exercise 2
```bash
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/footer)
$ git add service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/footer)
$ git commit -m "who to consult for the service"
[ft/footer 658fd6e] who to consult for the service
 1 file changed, 19 insertions(+), 6 deletions(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/footer)
$ git add about.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/footer)
$ git commit -m "Email and telephone on about page"
[ft/footer 5c8c86a] Email and telephone on about page
 1 file changed, 2 insertions(+)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/footer)
$ git push origin ft/footer
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 805 bytes | 402.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 3 local objects.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/f
t/footer
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      ft/footer -> ft/footer

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/footer)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/squashing)
$ git merge --squash ft/footer
Updating b6a7060..5c8c86a
Fast-forward
Squash commit -- not updating HEAD
 about.html   |  2 ++
 service.html | 25 +++++++++++++++++++------
 2 files changed, 21 insertions(+), 6 deletions(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/squashing)
$ git log
commit b6a7060010487e2381583e5f4298b0103bfff657 (HEAD -> ft/squashing, origin/main,
git-copy/main, main)
Merge: c4b8190 fe5888c
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Mon May 22 23:26:03 2023 +0300

    Merge branch 'main' of https://github.com/UmutesiMMA/The-gym-git-exercise-soluti
ons

commit c4b819087dde7ae6aba4d62346f7bba4899433f5
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Mon May 22 23:22:12 2023 +0300

    slogan on home page

commit fe5888cb86c1897a9ebbb3432443e76eeb09a7fd
Author: UmutesiMMA <133501822+UmutesiMMA@users.noreply.github.com>
Date:   Mon May 22 23:13:49 2023 +0300

    b3 e2

commit 7b6219d0c99f9e3d757974dd650c8b9af6b77ff7
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Mon May 22 22:31:16 2023 +0300

    changes to home page

commit 1bc787ef3caebd5d55ebab2c125753920b2d1634
Author: UmutesiMMA <133501822+UmutesiMMA@users.noreply.github.com>
Date:   Sat May 20 00:58:03 2023 +0300

    B2/E2

commit 3c7d5510c081878f1cd856b2fd9c658983e9bc22
Author: umutesimagnificat@gmail.com <umutesimagnificat@gmail.com>
Date:   Sat May 20 00:23:31 2023 +0300

    changes on same line different branches

commit de9b1d9903afb32e519bd524da372bff3fb0dd6a
Merge: 1e2cd02 fac79a3
Author: UmutesiMMA <133501822+UmutesiMMA@users.noreply.github.com>
Date:   Thu May 18 16:19:49 2023 +0300

    Merge pull request #3 from UmutesiMMA/ft/bundle-2

    Service page added

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/squashing)
$ git commit -m " merge squash"
[ft/squashing 7820373]  merge squash
 2 files changed, 21 insertions(+), 6 deletions(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/squashing)
$ git commit --amend -m "footer changes squashing"
[ft/squashing 09d2934] footer changes squashing
 Date: Tue May 23 00:32:27 2023 +0300
 2 files changed, 21 insertions(+), 6 deletions(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/squashing)
$ git push origin ft/squashing
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 571 bytes | 285.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/f
t/squashing
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      ft/squashing -> ft/squashing

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/squashing)
$

```
### Bundle 5
## Exercise 1
```bash
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/squashing)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 1.85 KiB | 135.00 KiB/s, done.
From https://github.com/UmutesiMMA/The-gym-git-exercise-solutions
   b6a7060..7c51788  main       -> origin/main
Updating b6a7060..7c51788
Fast-forward
 README.md | 136 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 136 insertions(+)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add index.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git commit -m "home to index"
[main 55de024] home to index
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename home.html => index.html (100%)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 233 bytes | 233.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   7c51788..55de024  main -> main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$
```
## Exercise 2
```bash

user@DESKTOP-TQVNUUS MINGW64 ~
$ cd ~/Documents/TheGym/

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym
$ git clone https://github.com/UmutesiMMA/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 95
Receiving objects: 100% (107/107), 1.95 MiB | 1009.00 KiB/s, done.
Resolving deltas: 100% (5/5), done.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym
$ cd ~/Documents/TheGym/git-cafe-exercise

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (main)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (main)
$ git commit -m "place to restaurant"
[main fbb473b] place to restaurant
 1 file changed, 3 insertions(+), 3 deletions(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 339 bytes | 84.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/UmutesiMMA/git-cafe-exercise.git
   d1d3f9c..fbb473b  main -> main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (main)
$
```
### Bundle 6
## Exercise 1
```bash
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (main)
$ git switch -c ft/menu-page
Switched to a new branch 'ft/menu-page'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (ft/menu-page)
$ touch Menu.html
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (ft/menu-page)
$ git add Menu.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (ft/menu-page)
$ git commit -m "Menu update"
[ft/menu-page 15d68da] Menu update
 1 file changed, 73 insertions(+)
 create mode 100644 Menu.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (ft/menu-page)
$ git push
fatal: The current branch ft/menu-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/menu-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (ft/menu-page)
$ git push --set-upstream origin ft/menu-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 562 bytes | 140.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/menu-page' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/git-cafe-exercise/pull/new/ft/menu-page
remote:
To https://github.com/UmutesiMMA/git-cafe-exercise.git
 * [new branch]      ft/menu-page -> ft/menu-page
branch 'ft/menu-page' set up to track 'origin/ft/menu-page'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (ft/menu-page)
```

## Exercise 2
```bash
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (ft/menu-page)
$ git checkout -b bug-fix
Switched to a new branch 'bug-fix'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (bug-fix)
$ git add index-4.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (bug-fix)
$ git push
fatal: The current branch bug-fix has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin bug-fix

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (bug-fix)
$ git push --set-upstream origin bug-fix
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'bug-fix' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/git-cafe-exercise/pull/new/bug-fix
remote:
To https://github.com/UmutesiMMA/git-cafe-exercise.git
 * [new branch]      bug-fix -> bug-fix
branch 'bug-fix' set up to track 'origin/bug-fix'.
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (bug-fix)
$ git commit -m "bug fix"
[bug-fix b0b8783] bug fix
 1 file changed, 1 insertion(+), 1 deletion(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (bug-fix)
$ git push origin bug-fix
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 293 bytes | 146.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/UmutesiMMA/git-cafe-exercise.git
   15d68da..b0b8783  bug-fix -> bug-fix

```

### Exercise3
```bash
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (bug-fix)
$ git switch -c hot-fix
Switched to a new branch 'hot-fix'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (hot-fix)
$ git add index-4.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (hot-fix)
$ git commit -m "Telphone update"
[hot-fix c92abf6] Telphone update
 1 file changed, 1 insertion(+), 1 deletion(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/git-cafe-exercise (hot-fix)
$ git push origin hot-fix
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 296 bytes | 148.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'hot-fix' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/git-cafe-exercise/pull/new/hot-fix
remote:
To https://github.com/UmutesiMMA/git-cafe-exercise.git
 * [new branch]      hot-fix -> hot-fix



```
