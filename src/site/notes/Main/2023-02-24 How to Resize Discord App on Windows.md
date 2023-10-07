---
{"dg-publish":true,"permalink":"/main/2023-02-24-how-to-resize-discord-app-on-windows/","noteIcon":""}
---

#wordpress-repost #discord #tech-support #guides 
[[2023-02-24\|2023-02-24]]

## (Or: How do I make discord smaller than it’s smallest size?)

Just in case the reddit thread ever dies, I had to look it up again and the 6 year old fix really does still work. I’m very tired so I’m not putting more effort into this, but because I look for it so often, it seems worth preserving.

This is discord employee’s reply, and it works, even this far along.

> Hey gang, sorry you’re not fans of this change. There are a bunch of visual problems when you change the app to what we called “unsupported resolutions”, which is essentially anything less than what we’re forcing now. We believe that for the average user this will provide a better overall experience, but we are listening to feedback.  
> If this change really bothers you, I figured out a workaround. Apologies if you find it a little complicated, this is the best I could come up with.  
> If you go into the discordcanary folder, there should be a text file named “settings.json”. Open it with notepad. Add in “MIN_WIDTH”: 0, “MIN_HEIGHT”: 0, to settings.json, after the “IS_MINIMIZED” line, but before the “WINDOW_BOUNDS” line
> 
> [https://www.reddit.com/r/discordapp/comments/6shs9n/comment/dld24oi/](https://www.reddit.com/r/discordapp/comments/6shs9n/comment/dld24oi/)

That’s meant for the test client though. To make it work with the current one, the file you’re after is over in `X:\Users\<Your_user_name>\AppData\Roaming\Discord\settings.json`
![Pasted image 20231007001727.png](/img/user/Main/attachments/Pasted%20image%2020231007001727.png)

![Pasted image 20231007001851.png](/img/user/Main/attachments/Pasted%20image%2020231007001851.png)
Next, you’ll want close discord (through the taskbar) and add these two lines to settings.json, between “IS_MAXIMIZED” and “WINDOW_BOUNDS”. They must be on separate lines, as shown in the second picture.

```
"MIN_WIDTH": 0,
"MIN_HEIGHT": 0,
```

If you didn’t kill discord via the system tray/task manager, you’ll probably need to restart in order for this to take effect. Otherwise, relaunching discord should be enough.
