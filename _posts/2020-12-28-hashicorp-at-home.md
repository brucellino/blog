---
layout: post
title: "Home-made Hashicorp Pi"
description: "How I'm using Hashicorp on my pis"
headline: "They make it, I use it, it's that simple."
category: home-office
tags:
  [
    "CI-CD",
    "platform",
    "Hashicorp",
    "automation",
    "vault",
    "consul",
    "waypoint",
  ]
image:
  feature: "louis-hansel-shotsoflouis-CfsFfbdRK70-unsplash.jpg"
mathjax: false
---

# What the hell just happened

It's been a long year for all of us. As someone who used to take pride and
satisfaction in writing about their work on the internet, I look back at the
void I've produced with mixed feelings. On the one hand, I've achieved several
goals at work, but haven't had been able to write about it publicly. On the
other hand, the things I did for myself have been so reduced in scope to things
that only find useful that I have doubted this whole year that anyone would be
interested in reading -- including future me! In general, it has been a year of
internalisation and self-reflection, given what has just happened to the planet,
so I am not all that surprised this subdued desire to write about technical
work. I have found myself less able to agree with the sentiment that _anything_
I write on the internet is worth reading, since it always seems so trivial as
soon as I see it written down, as if it were a waste of everyone's time. I've
found myself jotting down thoughts and immediately deleting them, with a slight
admonishment echoing in subconscious: _"Nobody needs to hear this crap"_.

On the other hand, I have two diaries full of daily notes and journal entries
from the last years, so something wants to come out.

I do like to write. As with most of the physical ones in my body, the writing
muscle hasn't been exercised much in plague times, and it feels like it's
starting to atrophy -- as I can even now tell from the quality of this post. So,
even though I have nothing of greater interest to share, I return here to write
something be it solely for the pure sake of exercise.

## Home sweet home

It's always brave to make predictions about the next few posts one plans to
write. "This is the first in a series of posts about what I've done with my
Raspberry Pis", the first would optimistically open, but it would take just a
few moments for history to tell you that the next post in this touted "series"
would come more than a few months down the line and start something like "Yeah,
this was supposed to be about my Pis, but I have something else on my mind now."

Consider this a premature apology then, for future negligence, for I do indeed
have a series in mind, about what I have done and what I plan to do with my Pis.

Before continuing though, it's worth taking another look at my changed
situation. In the past I have always exclusively used public infrastructure and
shared resources, building things for others and in general for community use.
Whether this was working in a large collaboration during my time as a grad
student or postdoc physicist in Phobos or ALICE, or co-ordinator during my time
at the CSIR building the distributed computing infrastructure, the
considerations on what tools and methods were appropriate were always generalist
in approach.

Now, however, I work in the private sphere, both at work and at home; this is
more about what _I_ want. It feels almost rude to be writing with such a
personal view! While it's one thing to express one's opinion and position on a
matter, I find it strangely trivial and selfish to simply write "I want to do
this particular thing". "Who cares?", I can hear the internet respond -- not out
of some perceived impostor syndrome on my part, but out of genuine lack of
interest on that of the world.

Again, I proffer my apologies, internet. There is nothing of interest here for
you. This is purely mine now.

## A plural of Pis

_"Revenons a nos moutons"_

I have a home office now, that has seen my persistent, constant presence because
of the pandemic. For the greater part of 2020, I spent almost every waking hour
in it. Now, along with the change in scope of the job when I left EGI came an
increase in what one might call "personal time". I was determined to start
filling this time with activities that stimulated my mind and body --
woodworking, writing, learning the guitar. One of this activities was
technological tinkering.

I started trying to learn new languages, or improve my fluency in those I could
barely converse in, in particular Go. However, working solely in software seemed
somehow to be just _not enough_, I wanted something that forced me to actually
touch things that weren't a keyboard with my actual hands. I wanted a tactile as
well as a mental experience.

And so it came to be that I started a collection of
[Raspberry Pis](https://www.raspberrypi.org/).

### Pi Three the First

It started with a single Raspberry Pi 3 kit - case, power, the whole basic deal.
After booting it and putting it on the network I got that little thrill when a
new machine comes up. You know, the feeling of "hey, I made this!", but of
course that was immediately followed by "OK, now what?".

**I have a frikkin Ph.D.** in the frikkin nuclear physics, I have no right to
feel any sort of achievement for starting a single board computer in my home
office! But this was _my_ silly little computer and I _did_ feel a silly little
fuzz of accomplishment.

Moving on, I decided to put the poor thing to work by putting
[PiHole](https://pi-hole.net/) on it. This worked quite well until it started
interfering with the work VPN, and became a bit too unstable to reliably leave
on.

### Pi 4 the Sensening

The few months subsequent to that first experience saw little change, but there
was a nagging refrain in my brain, reminding me that I wanted a _tactile_
experience. I wanted things I could hold in my hand, touch, move around and
through the world. My attention alit on the
[SenseHAT](https://www.raspberrypi.org/products/sense-hat/) and "Yes!", I
thought, "this thing has actual sensors!". I bought one and a
[Raspberry Pi 4](https://www.raspberrypi.org/products/raspberry-pi-4-model-b/)
to power it.

This was more like it! Data! The environment! I could even use it to show the
kids how to pull the real world into the simulated one by measuring temperature,
humidity, orientation, _etc_ and making the LED matrix light up in response to
changes to the physical world.

The Pi4 and Sense HAT combo is probably what got me really hooked on a Pi garden
in my office. I started using it as a visual
[Pomodoro timer](https://francescocirillo.com/pages/pomodoro-technique). There
is a physical toggle switch to start, pause and reset the timer. Furthermore,
it's an actual physical, three-dimensional thing that occupies actual
three-dimensional space in my office, not just a rendering of an idea on a
screen that I'm persistently staring into. At one point, I had it hooked up to
speakers, over on the other side of my office so that I had to actually get up
and take a few steps when the timer ended, better enforcing the principles
behind the method.

So, now there were two.

### Lots of little things

This setup felt good, but lost a bit of momentum. I started browsing the
reseller websites, especially [Pimoroni](https://shop.pimoroni.com/). What else
was out there? I started wondering if I could start making things by combining a
few components. Of course, _one_ could make things - there are plenty of kits on
sale for making little electronic projects - but could _I_ make something. Like,
with a soldering iron? The last time I had soldered anything at all was in
second year physics and I really had no idea what I was doing.

I realised though that the only voice telling me that this was a stupid idea was
that one in my head, and that dude can be a dick sometimes. It still felt
strange to justify something like this to myself simply by retorting "because I
want to", but that is what I did.

I went out and bought a soldering iron, then shipped a few
[Pi-Zeros](https://shop.pimoroni.com/products/raspberry-pi-zero-w), batteries,
solar panels, LED strips and other fun stuff like
[Scroll HATs](https://shop.pimoroni.com/products/scroll-hat-mini) to myself.

Oh and another Raspberry Pi 3 with an
[e-Ink HAT](https://shop.pimoroni.com/products/inky-phat) for good measure.

Now there were 6 little computers of varying power and pose in my cosy office!

As I came to gaze upon them, that curious illusion came to occur where instead
of a set of individual items I came to see them as the system they could be. I
came to wonder: "What can I do with these _as a whole_"?

## Actual tools for actual fools

So it is that we come back to the start of the next level in our strange loop -
making actual use of these things for myself. At the risk of missing some
context, I will simply state that we use a good portion of the
[Hashicorp](https://www.hashicorp.com) stable at work. I touch
[Packer](https://packer.io) and [Terraform](https://terraform.io) code every day
to maintain and provision cloud infrastructure and assets, and use
[Vault](https://vaultproject.io) to secure the secrets on it.

Hashicorp's products have an ergonomic polish to them which makes them almost
irresistible to use. The documentation, tutorials and guides seem to understand
just what one means to achieve and in plain language seem to pull you towards
those goals. With this attitude, I've been a bit sad that I didn't have a better
understanding of the other products in their catalogue, in particular
[Consul](https://consul.io). [Nomad](https://nomad.io) too intrigued me, but I
just couldn't see what they were _for_. When
[Waypoint](https://waypointproject.io) and
[Boundary](https://boundaryproject.io) came out this year, I watched eagerly and
jumped right in with their demonstration uses, but I still couldn't seem to
clear the fog in my mind that lay between the description of these things and
what they were actually useful for.

That is, until I started needing some sort of method for organising, accessing
and delivering applications to my Pi garden...

When I reached that higher-level concept of "system", I started to see the need
for Consul.

Nomad and Waypoint are next on my radar -- but since I've just managed to get
Consul deployed on my Pis, I wanted to stop here and take stock.

---

There is a nice symbiosis between work and private life, technologically
speaking. I have had to extend my knowledge of them, push them to see to what
extent they are useful in certain situations, what their true design was meant
to be, rather than simply rely on lazy habits I've formed over the years. As a
side note, this is true also for the _actual_ hardware tools in my office -- the
rotary tool, the saws, the soldering iron, the screwdrivers, the chisels and the
pincers. These are all made to be used in a certain way; when actually used as
intended, it is something akin to a sublime pleasure to feel them achieve what
that intent.

Having a little private workshop to try these things out in is, I find, very
useful in honing my skill and is both personally and professionally satisfying.
