# Github Classroom Fix 'n Push

A little script to push Github Classroom feedback back to Github. 

Specifically it goes into each repository, changes the remote URL to the original version (instead of the token), adds and commits everything, pulls any changes and then pushes all changes back to github, and then moves onto the next repository.


It needs to be executed from the parent directory of all the assessments. ie, in the following directory setup, from `project1`:

```
assessments/
    project1/
        student1repo/
        student2repo/
        ...
```
You'll want to make sure git and awk work from the commandline before running it. Try running git -v  or awk -v to test if they're present. Also, perhaps also make sure you're in bash not zsh. (just write `bash` in the terminal).

It's rough and dirty, contains no checking, use at own risk without warranty!