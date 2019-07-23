
# General

You can find more info about gohugo here:

* [quick-start](https://gohugo.io/getting-started/quick-start/)
* [Static Local Website with Hugo (file:///)](https://github.com/gohugoio/hugo/issues/622)


You can get started quickly with the following commands:

    > hugo server -D
    > hugo --buildDrafts
    > hugo new posts/my-first-post.md


# Clone the original and submodules

[Git-Tools-Submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules)

    > git clone --recurse-submodules https://github.com/cs224/cs224-hugo-dev-blog-sources.git


Or more manually:

    > git clone https://github.com/cs224/cs224-hugo-dev-blog-sources.git
    > cd cs224-hugo-dev-blog-sources
    > git submodule init
    > git submodule update

## Fetch updates:

    > git submodule update --remote

Or more manually:

    > cd cs224-hugo-dev-blog-sources/themes/ananke
    > git fetch
    > git merge origin/master

## Working on submodules

    > cd cs224-hugo-dev-blog-sources/themes/ananke
    > git checkout master

Now

    > cd cs224-hugo-dev-blog-sources
    > git submodule update --remote --merge

Or if upstream also has changes:

    > git submodule update --remote --rebase

Pushing can be done via:

    > git push --recurse-submodules=check
