# Инструкция по работе с Git и удаленными репозиториями

## Работа с ветĸами

### Git branch
    * git branch* "options" [-r] | [-a] --merged --no-merged   
    * git branch* "options"  [-l] [-f] branch-name start-point  
    * git branch* "options"  [-r] (-d | -D) branch-name ...  
    * git branch* "options"  (-m | -M) [old-branch] new-branch  
    * git branch* "options"  (-c | -C) [old-branch] new-branch  
    * git branch* "options"  [-r | -a] [--points-at]  
    * git branch* "options"  [-r | -a] [--format]

### Git branch option
    *  -v, --verbose    show hash and subject, give twice for upstream branch
    *  -q, --quiet  suppress informational messages
    * -t, --track   et up tracking mode (see git-pull(1))
    * -u, --set-upstream-to upstream    change the upstream info
    * --unset-upstream      unset the upstream info
    * --color[=when]      use colored output
    * -r, --remotes         act on remote-tracking branches
    * --contains commit   print only branches that contain the commit
    * --no-contains commit  print only branches that don't contain the commit
    * --abbrev[<n]    use n digits to display object names

### Переключение между ветками
    * *git checkout* *название ветĸи* — переĸлючиться в ветĸу
    * *git checkout* -b *название ветĸи* — создать новую ветĸу и сразу в неё переĸлючиться 

 #### Опции для git checkout
    * git checkout [-q] [-f] [-m] [branch]
    * git checkout [-q] [-f] [-m] --detach [branch]
    * git checkout [-q] [-f] [-m] [--detach] commit
    * git checkout [-q] [-f] [-m] [[-b|-B|--orphan] new-branch] [start-point]
    * git checkout [-f|--ours|--theirs|-m|--conflict=<style][tree-ish] [--] pathspec
    * git checkout [-f|--ours|--theirs|-m|--conflict=<style] [tree-ish --pathspec-from-file=file [--pathspec-file-nul]
    * git checkout (-p|--patch) [tree-ish] [--] [pathspec​] 