$ mkdir merged_repo
$ cd merged_repo
$ git init 
$ touch README.md
$ git add .
$ git commit -m "Initialize new repo"
$ git remote add -f first_repo `link_to_first_repo`
$ git merge --allow-unrelated-histories first_repo/master
$ mkdir first_repo
$ mv * first_repo/
$ git add .
$ git commit -m "Move first_repo files to first_repo directory"
$ git remote add -f second_repo `link_to_second_repo`
$ git merge --allow-unrelated-histories second_repo/master
$ git merge --continue
