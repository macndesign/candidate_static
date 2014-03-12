Candidate Site
==============

Website for candidates of the 2014 elections



For update gh-pages
-------------------

    git checkout master
    git status
    git commit -am "Committing changes to master"
    git push origin master
    git checkout gh-pages
    git rebase master # or merge, whatever your preference
    git push origin gh-pages
    git checkout master



Or auto in .git/config, in the [remote “origin”] section
--------------------------------------------------------

    push = +refs/heads/master:refs/heads/gh-pages
    push = +refs/heads/master:refs/heads/master



Unpublishing a project page
---------------------------

    git push origin --delete gh-pages
