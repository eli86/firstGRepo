This project reflects a brief overview of Git and Github.  In the workshop, we reviewed syntax, some basic logic, and the site.


Below is a draft of what I did in the workshop.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Last login: Sat Nov 16 13:31:59 on ttys000
Lauren-Heards-MacBook-Pro:~ laurenheard$ cd ~/
Lauren-Heards-MacBook-Pro:~ laurenheard$ cd
Lauren-Heards-MacBook-Pro:~ laurenheard$ cd
Lauren-Heards-MacBook-Pro:~ laurenheard$ pwd
/Users/laurenheard
Lauren-Heards-MacBook-Pro:~ laurenheard$ mkdir GitThing
Lauren-Heards-MacBook-Pro:~ laurenheard$ cd GitThing/
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git init
Initialized empty Git repository in /Users/laurenheard/GitThing/.git/
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
#
# Initial commit
#
nothing to commit (create/copy files and use "git add" to track)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txt
fatal: pathspec 'hello_world.txt' did not match any files
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ touch hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
#
# Initial commit
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	hello_world.txt
nothing added to commit but untracked files present (use "git add" to track)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
#
# Initial commit
#
# Changes to be committed:
#   (use "git rm --cached <file>..." to unstage)
#
#	new file:   hello_world.txt
#
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m 'First commit. Added hello world to repo.'
[master (root-commit) 69a10ce] First commit. Added hello world to repo.
 0 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
# Changes not staged for commit:
#   (use "git add <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#	modified:   hello_world.txt
#
no changes added to commit (use "git add" and/or "git commit -a")
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -a
error: There was a problem with the editor 'vi'.
Please supply the message using either -m or -F option.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
# Changes not staged for commit:
#   (use "git add <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#	modified:   hello_world.txt
#
no changes added to commit (use "git add" and/or "git commit -a")
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add .
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m "made chg within content.
> git status
> "
[master 9a4a351] made chg within content. git status
 1 files changed, 1 insertions(+), 0 deletions(-)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit 'What are you going to do next'
error: pathspec 'What are you going to do next' did not match any file(s) known to git.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add "What will you do next?"fatal: pathspec 'What will you do next?' did not match any files
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m 'make 2nd chg'
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -a '2nd change'
fatal: Paths with -a does not make sense.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m '2nd chg'
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add 'hello_world.txt'
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m 'another chg'
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m 'a change'
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git log
commit 9a4a351855fb08bf0241afcbec9601bcf808e688
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:04:15 2013 -0600

    made chg within content.
    git status

commit 69a10ce310c0e0725aeda7abb4f157fd4b6e6eea
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:00:13 2013 -0600

    First commit. Added hello world to repo.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ q
-bash: q: command not found
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m 
error: switch `m' requires a value
usage: git commit [options] [--] <filepattern>...

    -q, --quiet           suppress summary after successful commit
    -v, --verbose         show diff in commit message template

Commit message options
    -F, --file <file>     read message from file
    --author <author>     override author for commit
    --date <date>         override date for commit
    -m, --message <message>
                          commit message
    -c, --reedit-message <commit>
                          reuse and edit message from specified commit
    -C, --reuse-message <commit>
                          reuse message from specified commit
    --fixup <commit>      use autosquash formatted message to fixup specified commit
    --squash <commit>     use autosquash formatted message to squash specified commit
    --reset-author        the commit is authored by me now (used with -C-c/--amend)
    -s, --signoff         add Signed-off-by:
    -t, --template <file>
                          use specified template file
    -e, --edit            force edit of commit
    --cleanup <default>   how to strip spaces and #comments from message
    --status              include status in commit message template

Commit contents options
    -a, --all             commit all changed files
    -i, --include         add specified files to index for commit
    --interactive         interactively add files
    -o, --only            commit only specified files
    -n, --no-verify       bypass pre-commit hook
    --dry-run             show what would be committed
    --short               show status concisely
    --branch              show branch information
    --porcelain           machine-readable output
    -z, --null            terminate entries with NUL
    --amend               amend previous commit
    --no-post-rewrite     bypass post-rewrite hook
    -u, --untracked-files[=<mode>]
                          show untracked files, optional modes: all, normal, no. (Default: all)

Lauren-Heards-MacBook-Pro:GitThing laurenheard$ gitk

q

^C
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m "hello_world.txt"
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ gitk
^C
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m "trying something different"
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m "2nd chg to try using commit"
[master 5d7d937] 2nd chg to try using commit
 1 files changed, 1 insertions(+), 0 deletions(-)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git log
commit 5d7d93717ef8b1d8b6100e5ac2e1e4978136a0b0
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:18:49 2013 -0600

    2nd chg to try using commit

commit 9a4a351855fb08bf0241afcbec9601bcf808e688
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:04:15 2013 -0600

    made chg within content.
    git status

commit 69a10ce310c0e0725aeda7abb4f157fd4b6e6eea
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:00:13 2013 -0600

    First commit. Added hello world to repo.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ gitk
^C
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ change hello_world.txt
-bash: change: command not found
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ change hello_world.txt
-bash: change: command not found
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txtLauren-Heards-MacBook-Pro:GitThing laurenheard$ change hello_world.txt
-bash: change: command not found
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	modified:   hello_world.txt
#
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m "replaced text of 2nd line"
[master 4ce514c] replaced text of 2nd line
 1 files changed, 1 insertions(+), 1 deletions(-)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ change hello_world.txt
-bash: change: command not found
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git checkout hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git checkout hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git checkout hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txtLauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m "made chgs to text"
[master ac12fc7] made chgs to text
 1 files changed, 4 insertions(+), 2 deletions(-)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ get add hello_world.txt
-bash: get: command not found
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git reset HEAD hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git checkout hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git checkout hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m "Added text"
[master 65a005d] Added text
 1 files changed, 2 insertions(+), 0 deletions(-)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git log--pretty=oneline
git: 'log--pretty=oneline' is not a git command. See 'git --help'.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git log-pretty=oneline
git: 'log-pretty=oneline' is not a git command. See 'git --help'.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git log --pretty=oneline
65a005d5c3fb25df874142aba2ab2c0b53f0d5ed Added text
ac12fc73a8c2260ceb0336032d842b30d1a5d18b made chgs to text
4ce514ccde588080cfee5285238cebbdb96b6e50 replaced text of 2nd line
5d7d93717ef8b1d8b6100e5ac2e1e4978136a0b0 2nd chg to try using commit
9a4a351855fb08bf0241afcbec9601bcf808e688 made chg within content. git status
69a10ce310c0e0725aeda7abb4f157fd4b6e6eea First commit. Added hello world to repo
...skipping...
65a005d5c3fb25df874142aba2ab2c0b53f0d5ed Added text
ac12fc73a8c2260ceb0336032d842b30d1a5d18b made chgs to text
4ce514ccde588080cfee5285238cebbdb96b6e50 replaced text of 2nd line
5d7d93717ef8b1d8b6100e5ac2e1e4978136a0b0 2nd chg to try using commit
9a4a351855fb08bf0241afcbec9601bcf808e688 made chg within content. git status
69a10ce310c0e0725aeda7abb4f157fd4b6e6eea First commit. Added hello world to repo
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
 ESCOC
 Added text
 made chgs to text
 replaced text of 2nd line
 2nd chg to try using commit
 made chg within content. git status
 First commit. Added hello world to repo.
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
 ESCOC





.
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
 ESCOC






~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
 ESCOC






~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
 ESCOD






~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
 ESCOD





.
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
 ESCOD
 Added text
 made chgs to text
 replaced text of 2nd line
 2nd chg to try using commit
 made chg within content. git status
 First commit. Added hello world to repo.
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
 ESCOD
65a005d5c3fb25df874142aba2ab2c0b53f0d5ed Added text
ac12fc73a8c2260ceb0336032d842b30d1a5d18b made chgs to text
4ce514ccde588080cfee5285238cebbdb96b6e50 replaced text of 2nd line
5d7d93717ef8b1d8b6100e5ac2e1e4978136a0b0 2nd chg to try using commit
9a4a351855fb08bf0241afcbec9601bcf808e688 made chg within content. git status
69a10ce310c0e0725aeda7abb4f157fd4b6e6eea First commit. Added hello world to repo
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git revert [69a10ce310c0e0725aeda7abb4f157fd4b6e6eea]
fatal: ambiguous argument '[69a10ce310c0e0725aeda7abb4f157fd4b6e6eea]': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git revert [HASH]
fatal: ambiguous argument '[HASH]': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git log --pretty=oneline65a005d5c3fb25df874142aba2ab2c0b53f0d5ed Added text
ac12fc73a8c2260ceb0336032d842b30d1a5d18b made chgs to text
4ce514ccde588080cfee5285238cebbdb96b6e50 replaced text of 2nd line
5d7d93717ef8b1d8b6100e5ac2e1e4978136a0b0 2nd chg to try using commit
9a4a351855fb08bf0241afcbec9601bcf808e688 made chg within content. git status
69a10ce310c0e0725aeda7abb4f157fd4b6e6eea First commit. Added hello world to repo
--...skipping...
65a005d5c3fb25df874142aba2ab2c0b53f0d5ed Added text
ac12fc73a8c2260ceb0336032d842b30d1a5d18b made chgs to text
4ce514ccde588080cfee5285238cebbdb96b6e50 replaced text of 2nd line
5d7d93717ef8b1d8b6100e5ac2e1e4978136a0b0 2nd chg to try using commit
9a4a351855fb08bf0241afcbec9601bcf808e688 made chg within content. git status
69a10ce310c0e0725aeda7abb4f157fd4b6e6eea First commit. Added hello world to repo
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git log --pretty=oneline
65a005d5c3fb25df874142aba2ab2c0b53f0d5ed Added text
ac12fc73a8c2260ceb0336032d842b30d1a5d18b made chgs to text
4ce514ccde588080cfee5285238cebbdb96b6e50 replaced text of 2nd line
5d7d93717ef8b1d8b6100e5ac2e1e4978136a0b0 2nd chg to try using commit
9a4a351855fb08bf0241afcbec9601bcf808e688 made chg within content. git status
69a10ce310c0e0725aeda7abb4f157fd4b6e6eea First commit. Added hello world to repo
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git revert 65a005d5c
[master 8c1fa68] Revert "Added text"
 1 files changed, 0 insertions(+), 2 deletions(-)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
nothing to commit (working directory clean)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git log
commit 8c1fa68c4ef751c252d11e52f965433db7e3f4a9
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:53:09 2013 -0600

    Revert "Added text"
    
    This reverts commit 65a005d5c3fb25df874142aba2ab2c0b53f0d5ed.

commit 65a005d5c3fb25df874142aba2ab2c0b53f0d5ed
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:44:48 2013 -0600

    Added text

commit ac12fc73a8c2260ceb0336032d842b30d1a5d18b
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:36:29 2013 -0600

    made chgs to text

commit 4ce514ccde588080cfee5285238cebbdb96b6e50
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:32:02 2013 -0600

    replaced text of 2nd line

commit 5d7d93717ef8b1d8b6100e5ac2e1e4978136a0b0
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:18:49 2013 -0600

    2nd chg to try using commit

commit 9a4a351855fb08bf0241afcbec9601bcf808e688
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:04:15 2013 -0600

    made chg within content.
    git status

commit 69a10ce310c0e0725aeda7abb4f157fd4b6e6eea
Author: Lauren H <mslheard@gmail.com>
Date:   Sat Nov 16 14:00:13 2013 -0600

    First commit. Added hello world to repo.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ 
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git touch simple.txt
git: 'touch' is not a git command. See 'git --help'.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ touch simple.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add simple.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git reset simple.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ touch temp.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add temp.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	new file:   temp.txt
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	simple.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git rm temp.txt
error: 'temp.txt' has changes staged in the index
(use --cached to keep the file, or -f to force removal)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ rm temp.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	new file:   temp.txt
#
# Changes not staged for commit:
#   (use "git add/rm <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#	deleted:    temp.txt
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	simple.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ touch temp.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add temp.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m 'add new file'
[master d1f46de] add new file
 0 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 temp.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git rm temp.txt
rm 'temp.txt'
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	deleted:    temp.txt
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	simple.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git touch temp2.txt
git: 'touch' is not a git command. See 'git --help'.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ touch temp2.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	deleted:    temp.txt
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	simple.txt
#	temp2.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	deleted:    temp.txt
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	simple.txt
#	temp2.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ cd
Lauren-Heards-MacBook-Pro:~ laurenheard$ cd GitThing
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ cd hello_world.txt
-bash: cd: hello_world.txt: Not a directory
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git checkout -b v2
D	temp.txt
Switched to a new branch 'v2'
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch v2
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	deleted:    temp.txt
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	simple.txt
#	temp2.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m "new chgs"
[v2 5ecd87a] new chgs
 0 files changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 temp.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch v2
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	simple.txt
#	temp2.txt
nothing added to commit but untracked files present (use "git add" to track)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m "back to hello world"
# On branch v2
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	simple.txt
#	temp2.txt
nothing added to commit but untracked files present (use "git add" to track)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git branch
  master
* v2
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git checkout master
Switched to branch 'master'
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git merge v2
Updating d1f46de..5ecd87a
Fast-forward
 0 files changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 temp.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git checkout master
Already on 'master'
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git status
# On branch master
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	simple.txt
#	temp2.txt
nothing added to commit but untracked files present (use "git add" to track)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git remote add origin https://github.com/eli86/firstGRepo.git
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git push -u origin master
Username: 
Password: 
error: The requested URL returned error: 503 while accessing https://github.com/eli86/firstGRepo.git/info/refs

fatal: HTTP request failed
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git push -u origin masterUsername: 
Password: 
Counting objects: 22, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (12/12), done.
Writing objects: 100% (22/22), 1.89 KiB, done.
Total 22 (delta 3), reused 0 (delta 0)
To https://github.com/eli86/firstGRepo.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git add hello_world.txt
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git commit -m 'chg'
# On branch master
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	simple.txt
#	temp2.txt
nothing added to commit but untracked files present (use "git add" to track)
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ git push origin master
Username: 
Password: 
Everything up-to-date
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ touch README.md
Lauren-Heards-MacBook-Pro:GitThing laurenheard$ 
