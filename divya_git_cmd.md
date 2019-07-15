**Commands and operations** :
Created Repository
 * master
 * branch1
 * branch2

created a file Text.txt in branch1

* add - *echo 'Text' >fileName*  to add in local repo.
      *$ echo 'Text me'> TextMe.doc*

* add - *git add <Text.txt>*  to add in local repo.
      *$ echo 'Text me'> TextMe.doc
      $ git add TextMe.doc
      warning: LF will be replaced by CRLF in TextMe.doc.
      The file will have its original line endings in your working directory*

* commit - *git commit* - TO commit the last changes.
          *$ git commit --all -m 'new file added'
          [branch2 8cae9a0] new file added
           1 file changed, 1 insertion(+)
           create mode 100644 TextMe.doc*

* checkout - *git checkout master* - To change the branch
  *$ git checkout master
      Switched to branch 'master'
      Your branch is up to date with 'origin/master'.*

* branch - *git branch* - Give list of all branches with master
      *$ git branch
          brach1
          branch1
          branch2
          master*

* clone - *git clone <cloud url of any repo>* - give copy of cloud repo into local.
          *$ git clone https://github.com/divyaIntegrify/MyFirstGitProject.git
          Cloning into 'MyFirstGitProject'...
          remote: Enumerating objects: 55, done.
          remote: Counting objects: 100% (55/55), done.
          remote: Compressing objects: 100% (38/38), done.
          remote: Total 55 (delta 15), reused 25 (delta 3), pack-reused 0
          Unpacking objects: 100% (55/55), done.*

* Fork - it is on cloud - fork any repo on Git and it will give the copy of that repo in ur git repo

* HEAD-  *git reset HEAD* it Heads to your last Unstaged directory.Here reset cmd is for reset the not commited file.
          *$ git reset HEAD~
          Unstaged changes after reset:
          M       Text2.txt*

          *git revert HEAD*
          *$ git revert HEAD~
          [branch2 1bc7965] Revert "added text"
          1 file changed, 1 deletion(-)*

* merge- *git merge branch2* - it merge the branch2 into the current branch.
        *$ git merge branch1
        Merge made by the 'recursive' strategy.
        branch1_File.txt | 4 +++-
        text1.txt        | 1 +
        text2.txt        | 1 +
        3 files changed, 5 insertions(+), 1 deletion(-)*

* pull- *git pull* - pull update from github to local Repository
    *$ git pull
    remote: Enumerating objects: 12, done.
    remote: Counting objects: 100% (12/12), done.
    remote: Compressing objects: 100% (10/10), done.*

* add remote- *git remote add <url>* - it gives you remote repos in ur local.
          *$ git push --set-upstream origin Branch1
            Enumerating objects: 8, done.
            Counting objects: 100% (8/8), done.
            Delta compression using up to 4 threads*

* status- *git status* - Give status of files and directory
          *$ git status
            On branch Branch1
            Your branch is up to date with 'origin/Branch1'.
            nothing to commit, working tree clean*

* Log- *git log* - this cmd displays made changes by author with name,date and message

            *$ git log --oneline
              02faea6 (HEAD -> master, origin/master, origin/HEAD) Update divya_git_cmd.md
              8ec8a0e Add files via upload
              c76d386 Add files via upload
              6cdc72b Merge pull request #1 from divyaIntegrify/branch2
              af4b71f Merge branch 'branch2' of https://github.com/divyaIntegrify/MyFirstGitPr
              oject into branch2
              9c84a64 text22.txt updated
              1321a77 branch 2 file added
              9e23b3b PullFIle.txt
              6718f36 Updated
              f60a984 Merge branch 'branch1' into branch2*

* Tag- *git tag* - it gives list of all tags given by us. tag is used to mark any specific functionality in Repository.
          *$ git tag Tag1
          $ git tag -a v1.4
          *git tag
          $ git tag
          Tag1
          v1.4*


* fetch - It download all directory or tags of any Repository from github to our local git.
          *git fetch --all*  
          *git fetch --tags*
          *git fetch <url>*
