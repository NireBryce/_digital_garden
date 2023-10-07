---
{"dg-publish":true,"permalink":"/main/2023-02-26-i-had-to-figure-out-how-to-make-telegram-on-windows-not-have-arbitrary-window-size-minimums/"}
---

#telegram #tech-support #guides #cohost-repost 
[[2023-02-26\|2023-02-26]]

here's the solution so you don't have to

1. figure out where telegram is installed. this can be hard if you installed it through the microsoft store. So cheat -- ctrl-shift-escape to bring up task maanger, in either the processes (4 squares icon) or details tab, find telegram (hold ctrl if things are jumping around), then expand, click the telegram below it, right click, `"open file location"`
    
2. open command prompt or powershell, copy the address bar for that folder, then do
    

```
> cd location/of/the/telegram/folder
>  ./telegram.exe --scale XX where XX is the scale value you want
```

3. use the in-app scaling UI that now has extra values on it

thats it.

full credit goes to [https://www.journeybytes.com/telegram-desktop-custom-interface-scale/](https://www.journeybytes.com/telegram-desktop-custom-interface-scale/), all I did was add how to find the folder location