---
layout: post
title: TILvids Update - November 2022
---

![image](https://user-images.githubusercontent.com/69435791/201528671-d474b844-05cb-473e-8ad3-33ea4c489f44.png)

Hello! It's been a while since we've had a [TILvids](https://tilvids.com) blog update. The reason for this is two-fold: first, trying to keep a log of everything that has happened and then find time to do a write-up is pretty time-consuming, and second, not every month brings big updates, so it's often hard to come up with something to say. However, the last few months have been quite eventful, so I thought it time to do another update. Here's what's been going on (including a note about federation at the end)!

### Hosting Update

First some very good news. After months of trying to get it to work, I was finally able to stand up a redundant mirror instance of TILvids, based in the US. When we switched out hosting providers before, we shifted from Canada to Germany for the hosting. While this ended up being great for EU-based viewers, it was a degraded streaming experience for users in NA. While hosting the main site in Germany still means it loads a bit slower for NA users, at least the HD streaming should be much smoother (which has so far been the experience I've heard).

The rules I set in place for redundancy seem to be working, and as of this time the vast majority of the content on the site is being successfully mirrored (see the image above). I continue to look at ways to improve our experience, so if you have ideas, feel free to [let me know on Mastodon](https://mstdn.social/@tilvids).

### Mastodon

Speaking of Mastodon, the last few weeks of [Elon Musk's general mishandling of Twitter](https://www.cnbc.com/2022/11/09/elon-musk-took-over-a-struggling-twitter-and-has-quickly-made-it-worse.html) have been [quite beneficial to the Mastodon community](https://www.reuters.com/technology/mastodon-what-is-social-network-hailed-twitter-alternative-2022-11-07/). Since we've had a TILvids presence for quite some time on Mastodon, that meant a big influx of users for us as well! It's so nice to be able to use this open/decentralized medium as a huge way of getting the word out about TILvids. I've had so many wonderful conversations sprout from the Mastodon community, and look forward to even further conversations in the future. Please feel free to [follow our Mastodon account](https://mstdn.social/@tilvids) and join in!

### New Creators

Every month brings new creators, but the last few months have been even more special than usual! We've had some really great new creators come on board, including:

- [TheLinuxExperiment](https://tilvids.com/c/thelinuxexperiment_channel)
- [Thunderbird](https://tilvids.com/c/thunderbird_channel)
- [GamingOnLinux](https://tilvids.com/c/gamingonlinux_channel)

I used to be able to list every new creator in these blog posts, but there's just too many coming online to do that now. I do try to call them out on Mastodon though, so make sure to follow our account if you want the latest updates!

### Patrons

Once again, as a result of more attention on Mastodon, we've also seen an uptick in patrons at TILvids in the last month. This is incredibly important as we grow, because costs are going up across the board. We were recently hit with an inflation increase by our host, we're having to expand storage space, and add redundancy servers for better performance. I'm often asked by new creators "how much storage space can I have", and the answer completely depends on the donations coming in from the community. The more donations we have, the more space we can give, and the more creators will be willing to contribute their content. It truly is a virtuous circle. Thank you SO MUCH to everyone who contributes their financial support, no matter the amount, to help our community continue to grow! If you're interested in contributing, you can [find our Patreon here](https://www.patreon.com/tilvids)

### Spam

As TILvids has grown in popularity, so have the reports of spammers posting comments on videos. It's sometihng I'm aware of, and doing my best to combat it, though the tools in PeerTube are pretty limited. I've turned on email verification for new accounts, added a few moderators, and we work on deleting comments/accounts as they come in. It has been suggested that I turn off account creation and manually approve all new accounts, but with over a dozen new requests coming in every day, that's not something that scales well. I'll keep thinking about the problem, and there's [a decent discussion going on at the PeerTube GitHub repo](https://github.com/Chocobozzz/PeerTube/issues/5336) with some ideas as well.

### Thoughts on Federation

And finally, some thoughts on Federation.

I'm often asked the question, "Why doesn't TILvids federate with other PeerTube instances?" I thought instead of having to answer this over and over, I'd just write something here to refer people to in the future.

In general, most people start a PeerTube instance for one of two reasons:

1. They want to be a general instance. They have rules about storage space and possibly some light content guidelines, but otherwise will let anyone join and share content.
2. They are a content creator and want to host their own content, and federate with the rest of the PeerTube fediverse so their content can be discovered.

These are both completely legitimate reasons for starting a PeerTube instance and I support them. That said, my goal with TILvids was to do something different.

Before I started TILvids, I actually created content pretty regularly; I started uploading videos to YouTube around 2006. Eventually, over time, I watched as the spirit of YouTube shifted, from many small creators sharing interesting niche content, to "influencers" chasing ads and sponsors. This is not what I was interested in, and I felt it ruined the YouTube community (I have similar feelings about the general Internet as well, and very much subscribe to the ["original sin" theory of the Internet](https://www.theatlantic.com/technology/archive/2014/08/advertising-is-the-internets-original-sin/376041/)).

So I began to consider what I might do to change that. Originally, I tried starting a video community called "Smartyflix" (this was around 2017) based around a white-label video hosting service. There were very few hosting solutions at the time, and it became prohibitively expensive to scale. My hope was that I could find enough people to pay for the service to keep it afloat, but that never materialized.

Disappointed but undeterred, I set the idea on the shelf for a while. Then a few years later, I started hearing about new hosting options beginning to come online. I took a look at LBRY but was immediately turned off by the crypto aspect, and found much of the content to be riddled with conspiracy-peddling garbage. I also discovered another ecosystem called PeerTube, and while it didn't have any of the crypto nonsense of LBRY, it still suffered from pretty low-quality content throughout the ecosystem. But I loved the decentralized spirit and self-hosting, which felt so much like the early years of the Internet.

From this, I saw an opportunity: What if I could leverage the potential of PeerTube, and find a way to limit the garbage content, to build a community of niche edutainment content that was similar to the early years of YouTube? I decided early on that this likely meant NOT becoming a "general" PeerTube instance, which also meant limiting the federation aspect, at least initially, so as to give the community time to define itself. As I talked to video creators and explained my idea, the federation concept was so foreign to them anyway that it only made more sense to simply ignore that aspect of it.

Which takes us roughly to today. I continue to believe that limiting the federation aspect of TILvids is important to how the community will grow. I have talked before about the ["hub and spoke" model of TILvids](https://blog.tilvids.com/TILvids-Update-May-2021/) as how I see us eventually embracing federation. As creators come to TILvids and grow, we will encourage them to start their own instances, and then federate with them. This can be viewed as a strong vetting process to who we choose to federate with (similar to choosing who to federate with as a general PeerTube instance). This is important to me as a creator, because I strongly believe it is in the best interest of creators to eventually control their means of hosting their content, while recognizing this is very challenging for early creators, and why something like TILvids is important to them. Over time, we'll grow a large ecosystem of edutainment content creators.

Hopefully that sheds some light onto the reasons behind this decision. I know that not everyone in the PeerTube ecosystem agrees with this strategy, and that's perfectly fine. Diversity of ideas is healthy for an open community, and this is just another of them. Time will tell if it will be a beneficial one.

### Parting Thoughts

This turned out to be a much longer post that I originally intended, but I suppose that's what happens when you don't post an update for a few months. Perhaps I'll try to put these out roughly quarterly in the future, depending on if people find the information useful/interesting. As always, I want to thank the entire TILvids community for everything. Your support, whether through donations, viewings, content contribution, or just spreading the word, is constantly appreciated by me. Our community is what you make of it, and so far, we've been making something great. Let's keep building! 💙
