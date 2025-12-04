---
slug: death-by-docusaurus
title: Death by Docusaurus (Almost)
authors: eric
tags: [selfhosting]
---

eric-post.com fought for it's life today. I don't think it will survive the git push that allows you to read this.

<!-- truncate -->

This domain is no longer using Ghost. Welcome to my new minimum viable product! 

[Docusaurus](https://docusaurus.io) is an open‑source static‑site generator.

I switched from cloud flare zero trust tunnels to Pangolin running on a private VPS. One big problem: Couldn't find a way to put an SSO/2FA in front of the /ghost route like I could with zero trust policies. Yucky. I stood up and said no to that. Ghost was already something I was happy to ditch but, like my first blog post hinted at, I also don't want to manage a codebase. Docusaurus promised to protect me from myself and force me down the tutorial/blog-like structure. Forcing me to keep a manageable code base as I go into the future. Ghost was too restrictive, but maybe this will hit the sweet spot? I think probably.

[Pangolin](https://github.com/fosrl/pangolin) is a self-hosted tunneled reverse proxy server with built-in [crowdsec](https://github.com/crowdsecurity/crowdsec). 

Why switch to Pangolin? Well, cloud flare has had its ups and downs lately, and I figure I could do much worse. Honestly, it just reminded me that there is an open source solution that I've heard a lot an of great things about. I just needed step outside my comfort zone and pick up a VPS to run it on (a requirement). A Black Friday miracle happened, and I remembered to take a look. RackNerd had something just fine for $18 a year.

My comfort zone has always been well within my own networks. A VPS always felt too extra. However, I had experimented with setting up tail scale on a Raspberry Pi running at my Mom's house several months back. I've been testing ideas for services I could host for my family. Stuff like photo albums. It then dawned on me that I could just lock down this VPS in almost every conceivable way and just run traffic through tailscale. I ran through the steps on this site [here](https://randomadult.com/secure-it-essential-vps-security-for-ubuntu-24-04-lts/) to sanity check my security expectations. It was an overall fun process.

[Tailscale](https://tailscale.com) is a zero‑config VPN that turns any device into a secure, private mesh network using WireGuard.

Tailscale is still magic to me right now. I'm still basking in its glow. I am thankful for its existence. I can see some slightly better, more open-source solutions out there, but I am cool with this.

I should point out that I wanted to post about Docusaurus. I failed pretty badly so far. I can see that. Maybe mention a few things about using GitHub pages and probably brag about finally getting my git actions to work. I push a button, eric-post.com updates. Noice!

In fact, I've experienced a lot of moments over the years that had me wondering why I think I could actually do any of this. Sometimes I decide to do a thing, and so I gave it a shot. This can lead to some cascading consequences, as that tends to happen, that turns a small project into a quagmire of quicksand. Felt stuck. I gave up many times but was always drawn back wondering "maybe this time!”. I can't help it. I think this post can at least illiterate that process. One solution leads to another until eventually I can see over the hill. Once I get to the top, it's easy to see the path I took. Meandering around and stuffed with digressions. 

Eric of two years back would think what I am doing now is almost sci-fi. Outside of something he could do. Eric now: It's no big deal. Just gotta learn this and that. Conquering these hills keep me addicted to my home-lab.