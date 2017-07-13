# Komendy Github


1. **_git status_** - pokazuje nam status naszego pliku np animals
```
MacBook-Pro-Szymon:animals szymondutka$ git status
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	animals
	mysz2.txt

nothing added to commit but untracked files present (use "git add" to track)
```


2. **_git pull_** - zbiera wszystkie zmiany ktore zostaly wprowadzone do glownego repo w githubie
```
MacBook-Pro-Szymon:animals szymondutka$ git pull
remote: Counting objects: 1, done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), done.
From https://github.com/szydut11/github
   5138b0f..af13bba  Animals    -> origin/Animals
Already up-to-date.
```


3. **_git push_** - wypycha nasze zmiany w repo na komputerze do głownego repo w githubie
```
git push origin master
Username for 'https://github.com': szydut11
Password for 'https://szydut11@github.com':
Counting objects: 2, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 235 bytes | 0 bytes/s, done.
Total 2 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/szydut11/github.git
   3a42523..fc8734d  master -> master
```


4. **_git clone_** - za pomoca tej komendy mozemy sklonowac nasze dotychczasowe prace na repo i uzyc na innym komputerze a potem za pomoca push wyslac do githuba do repo nasze zmiany
```
it clone https://github.com/szydut11/github.git
Cloning into 'github'...
remote: Counting objects: 5, done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 5 (delta 2), reused 4 (delta 1), pack-reused 0
Unpacking objects: 100% (5/5), done.
Checking connectivity... done.
```


5. **_git checkout master_** - zmienia brancha na takiego jakiego chcemy np z food na master
```
MacBook-Pro-Szymon:animals szymondutka$ git checkout master
Switched to branch 'master'
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

MacBook-Pro-Szymon:animals szymondutka$ git branch
  Animals
  food
* master
```


6. **_git checkout -b_** - dodaje nowego brancha
```
MacBook-Pro-Szymon:animals szymondutka$ git checkout -b "food"
Switched to a new branch 'food'

MacBook-Pro-Szymon:animals szymondutka$ git branch
  Animals
* food
  master
```


7. **_git commit -m "adds (nazwa)_** - dodajemy nowego commita
```
MacBook-Pro-Szymon:animals szymondutka$ git commit -m "adds dog.txt"
[Animals 5138b0f] adds dog.txt
 Committer: Szymon Dutka <szymondutka@MacBook-Pro-Szymon.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 dog.txt
```


8. **_git branch_** - pokazuje dostepne branche oraz ten na ktorym jestesmy 
```
MacBook-Pro-Szymon:animals szymondutka$ git branch
  Animals
* master
```


9. **_git add_** - dodaje pliki ktore mozemy potem zmieniac i kontrolowac
```
MacBook-Pro-Szymon:animals szymondutka$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	mysz.txt

nothing added to commit but untracked files present (use "git add" to track)
MacBook-Pro-Szymon:animals szymondutka$ git add mysz.txt
```


10. **_git remote add origin "link do githuba"_** - dodaje repo na naszym komputerze
```
MacBook-Pro-Szymon:animals szymondutka$ git remote add origin https://github.com/szydut11/github.git
MacBook-Pro-Szymon:animals szymondutka$ git push -u origin master
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 242 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/szydut11/github.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
```


11. **_git merge_** - przy uzyciu tej komendy mozemu uzupelnic innego brancha o inne pliki ktore ma inny branch
```
MacBook-Pro-Szymon:animals szymondutka$ git merge master
Merge made by the 'recursive' strategy.
 zebra.txt | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 zebra.txt
```


12. **_git init_** - za pomoca tego polecenia tworzymy nowy podkatalog
```
MacBook-Pro-Szymon:animals szymondutka$ git init
Reinitialized existing Git repository in /Users/szymondutka/Desktop/Projects/animals/.git/
```