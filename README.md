# git-split
**a simple script for splitting the git history of a file**

As source files grow larger, it can be desirable to split them into several more manageable files that correspond to reasonable logical units. Within a git repository, each new file should ideally retain the history of the file it was copied from.

For instance, if a file `foo.src` is to be split into `foo_bar.src` and `foo_baz.src`, we can use **git-split** to achieve this by performing the following steps:

    $ sh git-split.sh foo.src foo_bar.src
    $ git mv foo.src foo_baz.src

After these two steps, both files will have the same history as `foo.src`, and we can start deleting the content we don't need from them.




