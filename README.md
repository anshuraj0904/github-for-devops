# Github

# To merge conflicts
``` bash
    git merge <other_branch>/<their_branch>
    # Shows a conflict.
    git merge --abort
    # To abort the merge ongoing(not mandatory).
    git checkout --theirs <somefile.ext>
    # This above command is for if we want to keep their code/text/anything.
    git checkout --ours <somefile.ext>
    # This is for, if we want to keep our code/text/anything.

    git add .
    git commit -m "Message"


    git merge <other_branch>/<their_branch>
``` 


# To squash multiple commits to one:-
``` bash
    git rebase -i HEAD~n
    # n for last n commits.
    # This will open an editor, wherein we'll have to replace pick with squash for all other than the first pick.
    # Change it and save it.
    # A new Editor will open and then, we'll write a new commit-line, if we want to save that editor, and boom we're done.  
``` 


# This one's for the stash:-
``` bash
    # Suppose you are working in the dev dir and something breaks out in the main branch.
    # So, you'd want to switch to main, but uh oh, it says, you've made change in your code, do commit them first, but you do not want to.
    # It is over here, where git stash comes in to the picture.

    # So, how do you use it:-
    git stash 
    # This one puts away our changes for a moment.

    # Next, you can checkout to where the issue/error is and work on that problem, comeback and do a git stash pop(it'll will return the latest added stash).

    # Suppose, I was in the dev and the issue occured in the production branch, then:-
    git checkout production
    # Do the tasks there

    # come back to the dev branch:-
    git checkout dev

    # get back the stashed data and continue with the work:-
    git stash pop
    # And, you are back to where you left all.    
```