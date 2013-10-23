git-lt
======

A git plugin to allow using local branches for a remote svn repo. It's like
git-svn, but without keeping track of history locally.

    usage:
    git lt help  How do I use this thing?
    git lt init  Initializes a git repository with a gitignore and creates a
                 special mirror branch
    git lt pull  Fetch the latest svn commit and rebase the current branch.
    git lt push  Make an svn commit for the most recent git commit.
    git lt add   Add a file to the git and svn repos.
    git lt diff  Alias for svn diff, piped through a highlighter
    git lt blame Alias for svn blame.
    git lt commit  Perform an svn commit and run git lt pull
    git lt status  Alias for svn status --ignore-externals
    
    commands you probably won't need:
    git lt rebase  Rebases current branch to mirror branch
    git lt fetch   Updates mirror branch to latest svn commit
    git lt trash   Trash local branch
    git lt reset-all	Trash local branch and run git lt pull
