# all-Git-commands

## **Git commands**  
##   
## **This list will make you bulletproof with Git.**  
## **Let’s go section by section 👇**  
  
⸻  
##   
🧭** 1. Configuration & Help**  
  
**Command**	**Description**  
==git config==	Set or get configuration variables (user, email, editor, etc.)  
==git config --global user.name "Pari"==	Set username globally  
==git config --global user.email "pari@example.com"==	Set email globally  
==git config --list==	Show all configurations  
==git help==	Get help on any Git command  
==git help <command>==	Open detailed docs for a command  
  
  
⸻  
##   
📦** 2. Creating or Cloning Repositories**  
  
**Command**	**Description**  
==git init==	Create a new local repository  
==git clone <url>==	Copy a remote repository  
==git clone <url> <folder>==	Clone into a custom folder  
  
  
⸻  
##   
📂** 3. Basic Snapshotting (Tracking Changes)**  
  
**Command**	**Description**  
==git status==	Show current state (staged, unstaged, untracked files)  
==git add <file>==	Stage a file for commit  
==git add .==	Stage all changes  
==git diff==	Show unstaged differences  
==git diff --staged==	Show staged differences  
==git commit -m "message"==	Save staged changes as a commit  
==git commit -am "message"==	Add *and* commit all tracked files  
==git restore <file>==	Undo changes in working directory  
==git restore --staged <file>==	Unstage a file  
==git rm <file>	==Remove a file from tracking  
==git mv <old> <new>==	Rename or move a file  
  
  
⸻  
##   
🔄** 4. Branching & Merging**  
  
**Command**	**Description**  
==git branch==	List local branches  
==git branch <name>==	Create new branch  
==git branch -d <name>==	Delete branch (safe)  
==git branch -D <name>==	Force delete branch  
==git branch -m <new>==	Rename current branch  
==git switch <name>==	Switch branches (new command)  
==git switch -c <name>==	Create and switch  
==git checkout <name>==	Switch branch or restore files  
==git merge <branch>==	Merge another branch into current  
==git rebase <branch>==	Move/Replay commits on top of another branch  
==git merge --abort==	Abort a merge if conflicts occur  
==git rebase --abort==	Cancel a rebase  
==git rebase --continue==	Continue after fixing conflicts  
  
  
⸻  
##   
🌐** 5. Remote Repositories**  
  
**Command**	**Description**  
==git remote==	List remotes  
==git remote -v==	Show URLs of remotes  
==git remote add <name> <url>==	Add a new remote  
==git remote remove <name>==	Remove a remote  
==git fetch==	Download changes from remote (no merge)  
==git pull==	Fetch + merge remote changes  
==git pull --rebase	==Fetch + rebase  
==git push	==Upload commits to remote  
==git push -u origin <branch>==	Push and set upstream branch  
==git push -f==	Force push  
==git remote show <name>==	Show detailed info about a remote  
  
  
⸻  
##   
🕵️** 6. Inspection & Comparison**  
  
**Command**	**Description**  
==git log==	Show commit history  
==git log --oneline	==Condensed log  
==git log --graph --oneline --all==	Visual branch graph  
==git show <commit>==	Show details of a commit  
==git diff==	Compare changes  
==git diff <branch1> <branch2>==	Compare branches  
==git blame <file>==	Show who last modified each line  
==git shortlog==	Summarize commits by author  
  
  
⸻  
##   
🧹** 7. Undoing Changes**  
  
**Command**	**Description**  
==git reset==	Reset current HEAD  
==git reset --soft <commit>==	Move HEAD but keep changes staged  
==git reset --mixed <commit>==	Move HEAD and unstage changes  
==git reset --hard <commit>==	Discard all changes up to a commit  
==git revert <commit>==	Create a new commit that undoes a previous one  
==git clean -n==	Show which files would be removed  
==git clean -f==	Delete untracked files  
  
  
⸻  
##   
🧱** 8. Stashing (Temporary Saving)**  
  
**Command**	**Description**  
==git stash==	Save uncommitted changes temporarily  
==git stash list==	Show stashes  
==git stash apply==	Reapply latest stash  
==git stash apply stash@{n}==	Reapply specific stash  
==git stash drop==	Delete latest stash  
==git stash pop==	Apply and delete stash  
==git stash clear==	Remove all stashes  
  
  
⸻  
##   
🧮** 9. Tagging**  
  
**Command**	**Description**  
==git tag==	List tags  
==git tag <tagname>==	Create lightweight tag  
==git tag -a <tagname> -m "message"==	Annotated tag  
==git show <tagname>==	Show tag details  
==git push origin <tagname>==	Push a tag  
==git push origin --tags==	Push all tags  
==git tag -d <tagname>==	Delete local tag  
  
  
⸻  
##   
⚙️** 10. Advanced / Plumbing Commands**  
  
**Command**	**Description**  
==git reflog==	Show history of HEAD changes (lifesaver after mistakes)  
==git cherry-pick <commit>==	Apply one commit onto another branch  
==git bisect==	Binary search to find which commit introduced a bug  
==git archive==	Create a zip/tar of a repository  
==git submodule==	Manage submodules (repos inside repos)  
==git gc==	Cleanup unnecessary files  
==git fsck==	Verify repository integrity  
==git rev-parse==	Parse and display revision info  
==git describe==	Show human-readable name for a commit  
==git annotate==	Same as git blame (older form)  
==git notes==	Add or read notes attached to commits  
  
  
⸻  
##   
💼** 11. Collaboration & Workflow**  
  
**Command**	**Description**  
==git pull-request== *(via GitHub CLI)*	Create a pull request directly from terminal  
==git fetch upstream==	Get updates from original repo (in fork)  
==git merge upstream/main==	Merge updates into your fork  
==git remote add upstream <url>==	Link original repo to your fork  
==git rebase upstream/main==	Rebase your branch with latest upstream changes  
  
  
⸻  
##   
🧠** 12. Informational / Metadata Commands**  
  
**Command**	**Description**  
==git rev-list==	Show commit IDs in order  
==git cat-file==	View contents of Git objects  
==git ls-files==	List files tracked by Git  
==git show-branch==	Show branches and commits  
==git verify-commit==	Verify GPG signatures of commits  
==git verify-tag==	Verify tag signatures  
  
  
⸻  
##   
🧩** 13. Git Aliases (Custom Shortcuts)**  
  
You can define your own commands for convenience:  
  
```
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.br branch

```
git config --global alias.unpushed "log origin/main..HEAD --oneline"  
  
Then you can just run:  
  
```
git unpushed

```
  
## **to instantly see unpushed commits.**  
  
⸻  
##   
🚀** 14. GitHub CLI (Optional but Powerful)**  
  
If you install **[GitHub CLI (](https://cli.github.com/)**[gh**)**](https://cli.github.com/)**, you also get:**  
  
**Command**	**Description**  
==gh auth login==	Authenticate with GitHub  
==gh repo clone== <user>/<repo>	Clone directly  
==gh pr create==	Create a pull request  
==gh pr view==	View a PR  
==gh issue create==	Create an issue  
==gh issue list==	List all issues  
==gh repo view==	View repo info  
  
  
⸻  
  
## **That’s the full set of Git commands you’ll ever realistically use — from beginner to professional contributor.**  
## **You now have the complete map 🔥**  
