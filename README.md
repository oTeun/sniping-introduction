# Introduction to minecraft name sniping
*This page was last updated on 09/19/2021*

## Welcome
If you're here, I suppose you want to start sniping minecraft usernames, but have no idea where to start.
I have been in the sniping scene since 06/06/2020, being introduced by [xinabox](https://www.youtube.com/user/XinaboxGaming "xinabox").
In this tutorial I will help you start out sniping, and understand the difficulties coming with that.
When you are first introduced to the concept of sniping, you may expect being able to snipe any username, and hiding usernames from others in an attempt of having a better chance.
This is not the case, everyone knows which names are dropping when, using [namemc](https://namemc.com "namemc").

## Table of contents
- [Common terms](https://github.com/oTeun/sniping-introduction#common-terms "Common terms")
- [Status codes](https://github.com/oTeun/sniping-introduction#status-codes)
- [Ratelimits](https://github.com/oTeun/sniping-introduction#ratelimits)
- [Acquiring a bearer token](https://github.com/oTeun/sniping-introduction#acquiring-a-bearer-token)
- [List of snipers](https://github.com/oTeun/sniping-introduction#list-of-snipers)
- [How to use delays](https://github.com/oTeun/sniping-introduction#how-to-use-delays)
- [Where to acquire Virtual Private Servers](https://github.com/oTeun/sniping-introduction#where-to-acquire-virtual-private-servers)
- [How to find upcoming names](https://github.com/oTeun/sniping-introduction#how-to-find-upcoming-names)
- [Community servers](https://github.com/oTeun/sniping-introduction#community-servers)

## Donations
If you feel like showing your love and/or appreciation for this project, then you may donate at these addresses :)

#### Bitcoin: 1HbbiMH4XfSmsnfAnWC9LhGtd7QHTu8huf
#### Ethereum: 0xa2EEA432bAa8cFc8972ceB4080C0B57DdEc03303

## Common terms
In sniping, you may get thrown off by any of these terms. They are used a lot in the community discord servers, and may confuse you at first, but they are actually really simple.

- SFA: Semi-Full-Access. This is a type of mojang account that was not originally bought by the current owner. It was hacked in to and then bought by someone. Using these types of accounts to snipe with is not allowed, and not supported by anyone in the community. You will get hate for this

- MFA / FA: Mail-Full-Access / Full-Access. This account may or may not be originally bought from mojang by the current owner. The account is secured with access to the email linked to the account.

- TID: Transaction ID of the account

- OGE: The original email that the account was created with

- GC: giftcode / giftcard. This is currently the most loved method of sniping. The name will be sniped onto a new account without a username, making it a prename.

- prename: An account with only 1 name in the name history.

- delay: usually expressed in milliseconds, this is the time before the name drops that your sniper will start sending claim requests.

- API: application programming interface, the Mojang API is like a website that programs can send requests to, interacting with Mojang directly instead of via a website.

- namechange: sniping changing the name of an existing account.

- VPS: Virtual Private Server, it is like a computer that you can remotely access. People buy these to get better chance of sniping.

## Status codes
Most snipers show the response of a namechange request using a status code, I will list the most common status codes here:
- 200: successfully sniped the name
- 204: successfully sniped the name
- 400: the name is not currently available, your request was sent either too late or too early
- 401: unauthorized, the bearer token that you sent your request with is invalid
- 403: the name is not currently available, your request was sent either too late or too early
- 429: you have sent too many requests, and are currently ratelimited
- 502: the API is currently under high pressure, and was not able to return your request
- 503: the API is currently under high pressure, and was not able to return your request

## Ratelimits
When you send too many requests in a short amount of time, you will be ratelimited by the API.  
The ratelimits are as following:
- Namechange account ratelimit: you can send 3 namechange requests per account per minute
- Namechange IP ratelimit: you can send 2 namechange requests per IP per minute
- Giftcode account ratelimit: you can send 6 claim requests per account per minute
- Giftcode IP ratelimit: you can send 60 claim requests per account per minute
If you do not follow these limits, you will receive status code 429.

## Acquiring a bearer token
Some snipers require a bearer token in order to snipe.
In order to change the name of your account, Mojang needs to verify it is you who is sending the request (obviously).
To do this, the sniper sends a bearer token with the request.
This token grants almost full access to your account, so do not share it with anyone other than your trusted sniper program.
Usually, snipers can log in to your account using the credentials, but some snipers do not have this feature, and require your bearer token.
To acquire your bearer token, you may follow this tutorial made by [Kqzz](https://github.com/Kqzz "Kqzz"): [click here](https://kqzz.github.io/mc-bearer-token/ "click here")

## List of snipers
Now that you have a decent understanding of common terms and everything else that I have explained so far, let's list a few free snipers. I will give these snipers ratings based on personal experience.

### MCsniperPY
Link: https://github.com/MCsniperPY/MCsniperPY  
Website: https://mcsniperpy.com/  
Documentation: https://docs.mcsniperpy.com/  
YouTube tutorial: https://youtu.be/-y2ucB6FYq8  

- Easy to use: 8/10
- Easy to setup: 8/10
- Community: 10/10
- Support: 10/10
- Speed: 7/10
- Supports GC sniping: No
- Supports migrated accounts with Microsoft authenticating: No
- Supports namechange sniping: Yes

Discord server: https://discord.gg/MpxCuwQpR6  
Written in: Python  

> MCsniperPY has been the leading free open source name sniper since August 2020, and offers great support including documentation and tutorials.
It also currently has the largest sniping community discord server.

### MCsniperGO
Link: https://github.com/Kqzz/MCsniperGO  

- Easy to use: 8/10
- Easy to setup: 9/10
- Community: 10/10
- Support: 9/10
- Speed: 9/10
- Supports GC sniping: Yes
- Supports migrated accounts with Microsoft authenticating: Yes
- Supports namechange sniping: Yes

Discord server: https://discord.gg/MpxCuwQpR6  
Written in: Go  

> MCsniperGO was written by [the same developer](https://github.com/Kqzz "the same developer") that wrote MCsniperPY. It is faster than MCsniperPY, because it is written in Go.

### OneSnipe
Link: https://github.com/Geographs/OneSnipe  
Documentation: https://docs.onesnipe.xyz/  

- Easy to use: 8/10
- Easy to setup: 6/10
- Community: 5/10
- Support: 6/10
- Speed: 6/10
- Supports GC sniping: Yes
- Supports migrated accounts with Microsoft authenticating: Yes
- Supports namechange sniping: Yes

Discord server: N/A  
Written in: Python  

### Estime
Link: https://github.com/oTeun/Estime

- Easy to use: 8/10
- Easy to setup: 8/10
- Community: 6/10
- Support: 7/10
- Speed: 8/10
- Supports GC sniping: Yes
- Supports migrated accounts with Microsoft authenticating: Bearer token only
- Supports namechange sniping: Mojang only

Discord server: https://discord.gg/98ZMYfD9HJ  
Written in: Python  

### Yolo-Sniper
Link: https://github.com/Liza-Developer/Yolo-Sniper

- Easy to use: 6/10
- Easy to setup: 6/10
- Community: 8/10
- Support: 6/10
- Speed: 9/10
- Supports GC sniping: Yes
- Supports migrated accounts with Microsoft authenticating: Yes
- Supports namechange sniping: Yes

Discord server: https://discord.gg/dDB2f3FKYH  
Written in: Go  

### buckshot
Link: https://github.com/tropicbliss/buckshot  
Documentation: https://buckshot.netlify.app/  

- Easy to use: 8/10
- Easy to setup: 6/10
- Community: 5/10
- Support: 6/10
- Speed: 8/10
- Supports GC sniping: Yes
- Supports migrated accounts with Microsoft authenticating: Yes
- Supports namechange sniping: Yes

Discord server: N/A  
Written in: Rust  

### tango
Link: https://github.com/Miestrode/tango
> I'm not sure if this sniper still works, if I found out more info I will add it soon

## How to use delays
Coming soon, for now please watch this YouTube tutorial: https://youtu.be/xvO-tf5kHjo  

## Where to acquire Virtual Private Servers
> More will be added to this part soon

To get the most out of your sniper, it is **highly** recommended you use a Virtual Private Server, also referred to as VPS. You can buy those at websites such as [vultr](https://vultr.com "vultr") or [digitalocean](https://www.digitalocean.com/ "digitalocean")  
Referral links for discounts: 
- [digitalocean](https://m.do.co/c/82be9eef6593 "digitalocean")
- [vultr](https://www.vultr.com/?ref=8893010 "vultr")

Tutorial on how to use a VPS to setup a sniper is usually included on the sniper page. You should also watch this video: https://youtu.be/-y2ucB6FYq8

## How to find upcoming names
> More will be added to this part soon

The best way to find upcoming names is using [namemc](https://namemc.com "namemc"), click on "names" at the top of your screen, and sort by whatever you are looking for. The more views these names have, the more people will be going for them.

## Community servers
> A list of servers to interact with the sniping community. I sorted these servers by the popularity I have noticed.

- MCsniperPY: https://discord.gg/MpxCuwQpR6  
- Dismal: https://discord.gg/dDB2f3FKYH  
- Poseidon: https://discord.gg/FPfMqDyJms  
- Scythe: https://discord.gg/Nt9FazZG2x  

There are more discord servers, you can make a pull request if you would like to add on to this list

## Final word
If you have anything to add to this tutorial, please create a pull request. This took very long to make. Please donate. And good luck with sniping.  How to contact me:
- Email: teun@teun.lol
- Website: https://teun.lol/
- Discord server: https://discord.gg/98ZMYfD9HJ
- Discord tag: Teun#8740
