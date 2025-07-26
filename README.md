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