# DevSoc Subcommittee Recruitment: Platforms
Your task is to send a direct message to the matrix handle `@chino:oxn.sh` using the Matrix protocol. However, this message must be sent over a self hosted instance such as through the Conduwuit implementation or the slightly more complicated Synapse implementation.

For this to work your server must be federated, but you do not have to worry about specifics such as using your domain name as your handle (a subdomain will do!) or have other 'nice to have' features. Just a message will do!

**You should write about what you tried and your process in the answer box below.**

If you don't manage to get this working we'll still want to hear about what you tried, what worked and what didn't work, etc. Good luck!

---

> ANSWER BOX
```
I first started by looking up the matrix protocol, Conduwuit and Synapse, so I didn't just go in blind. After getting a basic understanding of them, I looked into Conduwuit first. I downloaded the Haswell-optimised binary needed for my machine but it kept coming up with errors so I decided to compile it myself using Nix (which I had to install first) and then built it. Now the problem arose when I wasn't able to create a Conduwuit user so I tried rebuilding the whole thing again which again didn't work. At this point, I decided to just keep going and see how far I could get. The next thing I did was setting up a systemd service where I had to change the exec start path since it wasn't in usr/bin/conduwuit (this made me think that perhaps the problem was that maybe my files were all over the place). This was the moment my laptop crashed and I didn't want to ruin my one-year-old laptop so I decided to stop here with Conduwuit.

I then deleted everything I did for Conuduwuit to try and use Synapse instead. For this to work, I first set up Docker and looked to download the required official synapse image and docker-compose file. The hurdle I hit here was with generating a valid configuration file because it just wasn't generating one. At this point, I wasn't sure if I just didn't understand what I was supposed to be doing or whether it was my laptops problem. As time was running out and I worked on this for quite a while, I decided to stop here for the sake of my sanity. I did learn quite a few new things through this process though which I never would have otherwise which was quite a nice experience.
 
```
