this is an experiment about branch
all the experiments procedures and results are recored here
* 2021/02/05 15:04: add this file, add, commit, push (f8fa5a)
* delete file on remote:
    *   2021/02/05 15:13: add "dead_file.txt", add, commit, push (2d6fc8)
    *   2021/02/05 15:15: delete "dead_file.txt" on remote (3fcfa0)
    *   2021/02/05 15:23: pull successifully, "dead_file.txt" is deleted successfully in local
* try to recue "dead_file.txt": 
    *   2021/02/05 16:50: git reset 2d6fc81, push, failed (Updates were rejected because the tip of your current branch is behind its remote counterpart.)
    *   2021/02/05 17:00: git push origin 2021_Feb --force, success, "dead_file.txt" appears on remote, but does not appear in local, pull still shows "already up to date" 
    *   2021/02/06 11:30: git status shows "deleted: dead_file.txt" changes not staged for commit
    *   2021/02/06 11:34: git checkout dead_file.txt and "dead_file.txt" appears in local folder. git status shows up to date with 'orgin/2021_Feb'
* try to rename this file:
    *   2021/02/06 11:45: rename this file on remote (0e5d1d)
    *   2021/02/06 11:48: pull successifully, this file is renamed to "exp.txt"

* delete file from local:
    *   2021/02/09 14:30: accidently merge 2021_Feb by master, and the "README.md" appears in branch 2021_Feb. Pull and "README.md" appears in local
    *   2021/02/09 15:00 rm "README.md", and git status appear "deletion: READ.md"
    *   2021/02/09 git add README.md, commit, push, successfully (note that if reset head to the earlier version, the file can be rescued)
* delete some contents in a file from remote:
    *   2021/02/18 delete a line from "dead_file.txt", commit
    *   2021/02/18 15:43 pull successifully, local file is changed
