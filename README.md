# Welcome to the Linux Chaos!

Wow, you stumbled into this pit of shell scripting madness! 🤯  
Congrats, you've just walked into a **highly chaotic, totally unorganized** mess that does the impossible...  
Or rather, just connects a **heavily restricted server** to the internet. Because why not? 🤷‍♂️

## What in the world is going on here?

So, if you see:
- **`Status: No`**  
  This is the calm before the storm. The server is OFF. It's not even *thinking* about coming online. 🙅‍♂️

- **`Status: Yes`**  
  **Boom!** We’re telling the server, “Wake up, daddy's home. Welcome home, son!” 💻🎉

- **`Stop: No`**  
  Nah, we’re not telling the server to stop. It’s just hanging out, doing its thing. ✌️

- **`Stop: Yes`**  
  Okay, it’s bedtime for the server. Time to shut it down like it's a Netflix binge session. 💤

## What’s happening behind the chaos?

Here’s the master plan (if you can call it that):
1. **Syncs with GitHub**: Because we just have to keep things *somewhat* updated. It stashes changes, pulls the latest from the repo, and pushes it back. It's like GitHub's version of "I don't know what’s going on, but I’m doing something!" 😎
2. **Monitors Services**: Running services? Oh, we’ll monitor them like they’re our kids. If one goes down, we resurrect it faster than you can say `sudo`. 🔄
3. **Starts Services**: Flip the switch, and BOOM, services (code-server & cloudflared) are running... like a rocket 🚀
4. **Stops Services**: If we get a “Stop” signal, we shut things down like it's the end of the world. Don’t worry, it’s all graceful. 💀

## How does this mess work?

1. It checks a file on GitHub (`status.txt`). If it says "Yes," the server wakes up. If it says "No," it’s basically a digital snooze button. 🛏️
2. If it sees `stop.txt` on GitHub, we stop services like it’s a hard stop in a race. 🚫
3. Syncs with GitHub, just to make sure we’re all living in the same universe... at least for now. 🌌
4. Every minute, it checks if the services are still running, because someone’s gotta do it. If not, the script just restarts them. No biggie. 🔄

## Important (and slightly terrifying) Notes

- **Status**: "Yes" means *we’re on*, "No" means *we’re off*. It’s that simple... or is it? 🤔
- **Stop**: If it’s "Yes," we’re saying "time’s up!" and shutting everything down like a bad party. 🛑

- **`link.txt`**: Oh, this file contains a special link... and don’t even think about accessing it without the password! It’s password-protected because Linux chaos needs boundaries (sort of). 🔐

## The Linux Way: Let's Break Things!

This is **absolute chaos**—nothing is smooth here. Things may break, services may crash, and you might just end up Googling "How to fix a server after running a shell script." 🤷‍♂️

But hey, it’s all part of the fun, right? This project is for the brave souls who dare to dive deep into the madness of Linux and shell scripting. Go ahead, push it to the limits, break things, and then fix them. Or don’t. 😂

> **Disclaimer**: If you actually try to use this in a production environment, well... good luck. It’s like handing a toddler a chainsaw and saying, "Do your thing!" 😅

> **Unless you're like me...** Then it’s just another **day**. 🔥
