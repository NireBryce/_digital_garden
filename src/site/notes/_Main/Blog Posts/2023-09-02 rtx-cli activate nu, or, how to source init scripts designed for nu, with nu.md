---
{"dg-publish":true,"permalink":"/main/blog-posts/2023-09-02-rtx-cli-activate-nu-or-how-to-source-init-scripts-designed-for-nu-with-nu/","noteIcon":""}
---

#rtx #rtx-cli #nushell #rustlang #rust #linux #shell
[[2023-09-02\|2023-09-02]]

Google returned nothing so here's this.

Nu has no eval(), which means you have to pipe the init script to a file like so:
```rtx-activate nu >> ~/.config/nushell/.rtx.nu```

The nu equivalent of `source` in bash/zsh is just `use`, and it's used in the same way as `source` in bash/zsh
```use ~/.config/nushell/.rtx.nu```

put these at the end of your config file, below the last bracket (usually the end of the env block, but I don't remember)