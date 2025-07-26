# Github

# To merge conflicts
``` bash
    git merge <other_branch>/<their_branch>
    # Shows a conflict.
    git merge --abort
    # To abort the merge ongoing.
    git log --diff
    git checkout --theirs <somefile.ext>
    # This above command is for if we want to keep their code/text/anything.
    git checkout --ours <somefile.ext>
    # This is for, if we want to keep our code/text/anything.

    git add .
    git commit -m "Message"


    git merge <other_branch>/<their_branch>
``` 