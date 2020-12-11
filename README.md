# dh2017.adho.org

This repo contains a static dump of the WordPress site that is/was serving dh2017.adho.org.

- The dump was generated using a version of the [Simply Static](https://wordpress.org/support/plugin/simply-static/) plugin that I modified to work with `php-7.4`.
- It was then processed to completely remove all the hardcoded links (although it seems unlikely that this would ever be hosted anywhere other than dh2017.adho.org, it doesn't hurt, and it made testing a lot easier).
- Additional assets that Simply Static missed (?) were added.
- Further links were regularized and relativized (with aggressive and gratuitous use of `ag`, `sed`, and `perl`).
- A couple of `mailto:` links that were broken on the original site were fixed.
- A note was added to links to `conftool.pro/dh2017` given that the latter no longer exists.
- Some unnecessary and obstructive cruft was removed from the `<head/>` of each page.
- The search widget was removed -- it won't work without a backend, and there doesn't seem to be much need for a move involved solution.
- A 404 page was added.

Note that the combined book of abstracts (`abstracts/DH2017-abstracts.pdf`) comes in at ~175mb, which is too large for git, so this repo makes use of [`git-lfs`](https://git-lfs.github.com/). If you want to clone this repo for any reason you'll need to install `git-lfs` first (see also: https://docs.github.com/en/free-pro-team@latest/github/managing-large-files/versioning-large-files).
