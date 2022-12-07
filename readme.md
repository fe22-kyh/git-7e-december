# 7e December

## Live-kod

[Live coding examples](live-coding/)

## Övningar

[Git bootcamp](exercise/git-bootcamp/README.md)

## Material

- [Markdown cheat sheet](https://www.markdownguide.org/cheat-sheet/)
- [Useful git commands](https://www.freecodecamp.org/news/10-important-git-commands-that-every-developer-should-know/)
- [Git setting up a repo](https://www.atlassian.com/git/tutorials/setting-up-a-repository)

## Git simple steps
Typiska steg för utvecklingsprocessen

### För varje ny projekt
1. git init
2. git branch -M main
3. git remote add origin <remote_repo_url>
  
Ifall du arbetar med andra så krävs det endast att en deltagar sätter upp ett remote repo med ovanstående kommandon, övriga deltagar använder kommandot
- git clone <remote_repo_url>

### För varje commit
1. git add .
2. git commit -m "a small descriptive commit message"

### När repot ska uppdateras

#### första gången
- git push -u origin main

#### från main branchen
- git push

#### från branchen <branch_name>
- git push origin <branch_name>

### När en ny feature (tillägg) ska utvecklas
- git checkout -b <new_branch_name>

### När den nya featuren ska läggas till i main
1. git checkout main
2. git merge <new_branch_name>

Obs! Det vanliga är att du först mergar in i en utvecklings branch där merge-conflicts hanteras, sen uppdateras main. Stegen för dev branchen och main branchen är detsamma.

