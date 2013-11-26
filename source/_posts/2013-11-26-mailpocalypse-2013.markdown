---
layout: post
title: "Mailpocalypse 2013"
date: 2013-11-26 12:42
comments: true
categories: 
---
I just solved the most confounding home IT mystery in recent memory, and I want to describe what happened. For two months, I have been receiving some, but not all email sent to me. At first, I didn't know I was missing any mail. But increasingly, people would see me and say "Hey, did you get my email about..." and I would just stare back in confusion. Sometimes, it would go the other way: I would wonder why so-and-so hadn't responded to me and wasn't that rude of them? I was starting to wonder if my mind was going way ahead of schedule.

If you have any experience with email, the first thing you'll think is "SPAM filter, dummy." Well, I do have some experience with email and I have a filtering setup that has been working great for me for over seven years. After checking all the reasonable locations for my missing messages, I started checking unreasonable locations, to no avail.

That's when I first spotted it: I was doing some work and my email inbox was partially visible in another window. A message that I would like to have read popped into view in the corner of my eye. I shifted my attention to it and one second later POOF, it was gone. Now I had proof that my messages were making it all the way to my machine before disappearing. I assumed it must have been moved somewhere I didn't intend. I searched everywhere: trash, spam, archives, pending, and any of a number of organizing boxes. I even tried grepping my email cache. It was just gone.

I tried turning off all my processing rules (including the SPAM filter). No change, messages still blinked out of existence within a few seconds. This was when I started suspecting one of my other devices. I have a desktop, a laptop (actually, it's my wife's, on which I have an account), a phone, and a tablet, all of which are capable of reading, composing, moving, and trashing email. I started turning them off one by one. This is what finally led me to the answer.

Every once in a while, I'll borrow my wife's MacBook Air when she's not using it and I need to be mobile. I have the same email setup on it as on my desktop machine (namely, Apple Mail and Michael Tsai's [SpamSieve](http://c-command.com/spamsieve/)). I ran afoul of [a problem](http://c-command.com/spamsieve/manual-ah/why-is-every-message-go) whereby SpamSieve's plugin for Mail became disabled, which prevents it from distinguishing between good mail and bad. Whenever the laptop received any messages, it would move _all_ of them to the Spam folder, which is a local directory (i.e. not shared over the network). Since all my accounts use IMAP, Apple Mail would dutifully update thier respective servers that the mail had been moved offline.

What was fiendish about this problem is that I would only miss messages when Mail was running on the laptop, and that was only once in a while. The silver lining is that all those missing messages were sitting safely in the laptop's Spam directory all along. My stomach rolled over this morning as I took inventory of everything over the past two months that I should have seen.

I sincerely apologize for any communications you were expecting from me and didn't get. After so many years of living and breathing computer stuff, I thought I was innoculated against anything as mundane as losing email. If you'll excuse me, I have a couple thousand messages to attend to.
