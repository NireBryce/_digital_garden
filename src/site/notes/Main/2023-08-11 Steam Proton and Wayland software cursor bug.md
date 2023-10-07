---
{"dg-publish":true,"permalink":"/main/2023-08-11-steam-proton-and-wayland-software-cursor-bug/"}
---

#linux #steam #steam-proton #planetside #wayland #chromium #bugs
[[2023-08-11\|2023-08-11]]

I don't have it in me to write a bug report or know if it's chromium or wayland, however, if you want to:

I'm running manjaro, with kde, with wayland

I had planetside2 crash under whatever the newest non-testing version of proton is

now _every chromium-based window_ that is on the monitor I was playing planetside on, has the planetside software cursor and is unclickable.

until I move it to a different monitor.

but when I move it back, the soft cursor problem is still there

it _only_ effects chrome windows, electron windows, and steam

and steam is built on chromium.

### update:

if I move where my monitor is in virtual space (to the left/right/top) of my other monitor in the monitor editor, it fixes it, until I move it back to that virtual position

did not persist through a reboot