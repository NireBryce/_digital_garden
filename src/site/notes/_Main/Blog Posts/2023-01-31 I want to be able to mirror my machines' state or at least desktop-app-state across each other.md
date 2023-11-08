---
{"dg-publish":true,"permalink":"/main/blog-posts/2023-01-31-i-want-to-be-able-to-mirror-my-machines-state-or-at-least-desktop-app-state-across-each-other/","noteIcon":""}
---

#white-whales #computers #machine-mirroring #open-source #linux #cohost-repost 
[[2023-01-31\|2023-01-31]]

I know it's impossible because computers have convergent state

and I get that open source development is generally just wherever the dopamine takes people, but the fact that I can't check "sync desktop session across devices" like I can to persist locally through a reboot, does feel like a glaring hole in everything with how device use has changed.

but I really do wish I could have my 3 machines reflect each other as I walk between them, without needing to use fucking remote desktop-style high latency high video demand stuff thanks to things like: WSL and iPadOS not supporting x-forwarding (ruling out 2/4 machines)

thin clients and terminal servers are a cool idea but pretty impossible to actually implement as a home user in the way I want, which is to be able to access the same desktop tasks (which is to say, My Working Memory). I can use tmux/zellij/mosh for terminal state, but I often need GUI for things like VSCode, or a web browser.

But I also just want all of my machines to _reflect the global state locally_. Which I understand is impossible. But the ideal is "everything uses my powerful desktop for compute-intensive tasks, but when it loses connection it can do everything locally, seamlessly, and git-merge with the main state". All of my Black Mirrors should go to the same place, until they need to not (latency no longer LAN, connection loss, etc)

So many of my usecases are basically terminal-to-mainframe archetecture and yet I have to be running an OS, it might as well reflect the thing I'm remoting into, so I can be doing the same thing whichever one I am at. But I can't use "remote desktop"-style streaming stuff here, because everything has a different resolution and nothing, and I mean NOTHING, handles that well without a lot of time wasted trying to make VNC (it's one of the few that WILL do custom resolutions on the host machine) have comfortable resolutions for every possible monitor orientation on every device.

I currently sync my browser tabs across devices semi-manually with Tab Outliner. Not just tabs, but categorized tabs, which windows have which tabs, etc. I use Zellij and Atuin and do most of everything by sshing into one server. But I shouldn't have to. The world has changed but OSes haven't, and while I understand these are hard and perhaps problems, we've got people working for months on making a browser run javascript a fractional percent faster (but not more efficiently) instead.

in the mean time, I'll keep dreaming about being able to easily contort nix into a long-orbit version of this (everything uses same base config, and then the filesystem is a NAS that everything copies when it's updated) but nix isn't ready for home users yet, not really. Unless you have a hobby worth of free time to spend to get up to speed.