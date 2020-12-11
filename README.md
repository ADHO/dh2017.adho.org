# dh2017.adho.org

This repo contains a static dump of the WordPress site that is/was serving dh2017.adho.org.

- The dump was generated using a version of the [Simply Static](https://wordpress.org/support/plugin/simply-static/) plugin that I modified to work with php 7.4.
- It was then processed to completely remove all the hardcoded links (although it seems unlikely that this would ever be hosted anywhere other than dh2017.adho.org, it doesn't hurt, and it made testing a lot easier).
- Additional assets that Simply Static missed (?) were added.
- Further links were regularized and relativized (with gratuitous use of `ag`, `grep`, `sed`, and `perl`).
- A couple of `mailto:` links that were broken on the original site were fixed.
- A note was added to links to `conftool.pro/dh2017` given that the latter no longer exists.
