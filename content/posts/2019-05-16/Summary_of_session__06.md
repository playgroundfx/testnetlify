+++
categories = ["Cryptocurrency", "Blockchain", "SmartContract"]
date = "2019-05-16"
description = "Summary of session #06"
tags = ["Cryptocurrency", "Blockchain", "SmartContract"]
title = "Summary of session #06"
type = "post"
+++

[![DApps Dev Club][1]][2]

[Sessions][3][Partners][4][Projects][5][Certificates][6]

[![Github][7]][8][![Discord][9]][10][![RSS Feed][11]][12]

# Summary of session #06

![][13]![][14]

 _Web3: Front-end setup + Web3.js scaffold + Smart contract
interactions: Queries, mutations, and listening to events_

The DApps Dev Club held its sixth session, about building front end web
applications that talk to [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s, on Tuesday evening at
Chainstack.

We spent some time covering general front end web development, and then
built upon that by introducing **web3 provider** s and **web3.js** ,
using that to talk to a [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/) instead.

~~Videos will be posted soon!~~ [Videos for this session][15] are now
available!

## Format

Continuing with the bar set in the previous sessions, this one was
almost entirely comprised of hands-on stuff, and very little theory from
a slide deck.

![Let me hit you with some knowledge][16]

Those who've attended our more recent sessions will know that we are
**not** doing this ^. It isn't about a speaker presenting information,
and the audience downloading that information. Instead, we're about
interactively trying out the things we talk about as we go along - less
talking and more doing.

## Difficulty and pace

This session's hands-on exercises turned out to be the most difficult
among all the sessions thus far, based on the feedback during and after
the session that I have got from you.

In previous sessions, usually about at least two-thirds of those
attending have managed to get the stuff working - and usually at least
two-thirds of those attending have their laptops open and are actively
participating, by following along with the hands-on exercises - so that
has been pretty good! a€¦ and of course thanks very much to those who
volunteered to help out among others during the session (see the next
section, **above and beyond** ), that enabled us to achieved this.

In this session, however, only about half of you managed to get your
DApps working up to the first half of the hands-on exercises, and only a
third of you managed to to get your DApps working at the end of the
hands-on exercises - based on shows of hands.

This is indicative that the difficulty and pace was too hard or fast,
and that I need to makes some changes in the upcoming sessions. (more on
this in the next section, **reflections**.)

## Above and beyond

A few of you who attend these sessions have really stepped up, going
from attending the sessions, to actively helping out.

Thanks [Gerald Nah][17] for helping out during the session, with setting
up the AV and helping out with the recordings. This was a last minute
arrangement, so thanks for being accommodating!

Thanks [Jack Ng][18] and [Arif Rahman][19]. Both of them helped many of
you out during the session, troubleshooting, and getting you unstuck at
the tricky parts! Also, for **reviewing** my hands-on materials prior to
the session, and giving me **detailed feedback** on it - which was
certainly put to good use!

You deserve a shout out for being awesome! ðŸ™ŒðŸ™Œ The session would
not have progressed as **smoothly** as it did without you!

## Reflections

This session, as mentioned earlier, did not have a satisfactory "got it
working" rate - significantly down from the previous sessions. Thus we
will take this into account, and slow down the pace of the sessions.

In this one, we have clearly pushed the limits of both the scope and the
complexity of the content that we are covering during the session. This
has been duly noted, and in future sessions, we will reverse this trend
by reducing and simplifying instead.

The next session, and the remaining ones, will still aim to cover the
same concepts as originally planned; however, the goal will no longer be
to demonstrate or build all of them in hands-on exercises. The hands-on
exercises will instead be reigned back, and instead be more like those
in sessions #03 and #04, where it felt like everyone was being
challenged, but not too much to the point that you were unable to get it
working.

Apart from the content that was being covered, there was another
significant hurdle, which was the installation of various dependencies.
In this session there were no new tools to install, so we were not
expecting this issue to crop up - but it still managed to!

So what's going to change here? For starters, instead of simply saying
"install these tools a€¦" prior to the sessions - which we have already
been doing in our pre-session announcement posts - we will also add "a€¦
and install these dependencies." That will solve the problem for those
of you who are keen, and can come to the session prepared with all the
necessary bits already good to go.

Next up we have another issue, which is that installing depndencies
really should not be that hard to do - most of the time we are dealing
with NodeJs packages distributed on npm. However, some of the stuff
builds NodeJs native modules, which require certain dependencies that
just work better on UNIX systems (like Mac or Linux). Those who are on
Windows will have a much harder time though - many of you encountered
errors that fundamentally were attributable to misconfigurations of the
`PATH` environment variable, or certain system binaries that are pre-
installed on most UNIX systems simply being missing. For those using
Windows, setting up a working development environment is harder, and
requires more effort beforehand. Please consider installing
[Powershell][20] or [Windows Subsystem for Linux][21] in order to follow
along more easily!

## Topics

### Front-end web development set up

  * [Deck][22]
  * [Hands-on][23]

In our very first section, we ditched [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s and DApp
development entirely, and instead focused purely on regular web
development: HTML, CSS, and Javascript.

We are building a DApp that runs in the browser, so there is a lot of
common ground between "regular" web development, and DApp development -
in fact, one might even think of front-end DApp development as web
development that happens to make use of a [Libra](https://www.playgroundfx.com/blog/libra-creator/)ry/ module called
web3.js!

Here we set up a basic NodeJs project with webpack to do both
development builds with hot reloading as well as production builds.

### web3.js scaffolding

  * [Deck][22]
  * [Hands-on][24]

Following on from the previous hands-on exercise, we turned our CApp
(centralised application) into a DApp (decentralised application), by
adding web.js.

That was merely the first step though, we explored the concept of a
**web3 provider** , which in our case was injected into the browser by
MetaMask, and [how to](https://www.playgroundfx.com/blog/forex-trading-how-to/) use **web3.js** to build a _bridge_ that allows
regular Javascript to talk to nodes on the Ethereum network.

Following this, we explored what truffle does behind the scenes when one
runs the **build** and **migrate** commands, with a focus on the
**compiled byte code** and the **deployed byte code**. This actually, in
retrospect, answers a question that was asked, but did not get enough
time to answer in the previous session (session #05 on testing smart
contracts). We used the contents of `builds/contracts` to construct a
Javascript wrapper for the [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/) that we have built during the
previous sessions. a€¦ and this is the thing through which we are able
to interact with the [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s in the subsequent hands-on
sections!

### Querying State of a Smart Contract

  * [Deck][25]
  * [Hands-on][26]

The first, and most straightforward way of interacting with a smart
contract is to query its state. The solidity compiler auto-generates
public accessor [functions](https://www.fintechee.com/tutorial-for-forex-trading/basic-functions/) for each public state variable that it
contains, and we simply have to use those.

The main take away here, which is a reiteration of something which was
stressed in the previous session (session #05 about testing smart
contracts), is that we should use `.call()` instead of `.send()`,
because we want to query a local copy of the [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/) - which
web3.js does automatically, no extra work required here - instead of
sending the same query to the network, which involves the computational
overhead of processing a transaction, and therefore needs to be paid for
using gas.

At this point we would have built something that we can actually call a
DApp for the first time in this entire series ðŸŽ‰ðŸŽ‰ðŸŽ‰
congratulations!

### Mutating State of a Smart Contract

  * [Deck][25]
  * [Hands-on][27]

The other main interaction that we have with [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s is when we
mutate its state - that is to call a function that modifies its state
somehow. We also explored this concept in the previous session, but the
state transitions (mutations) that we performed, were done
programmatically within tests. This time we're doing more or less the
same thing, but the interaction is done by a user of our web application
instead.

Here we're no longer just working with a local copy, since we need to
send transactions in order to modify state, so we use `.send()` (not
`.call()`). We also explored [how to](https://www.playgroundfx.com/blog/forex-trading-how-to/) estimate gas manually, and what
happens when you ignore the estimate and specify either too much or too
little gas.

We also examined the transaction data - what web3.js actually transmits
to the Ethereum network - and related that back to what we learnt in the
earlier sessions. This wasn't, technically, related to front-end DApp
development, but it was something that was fun to look at at this point,
and to round out some theoretical concepts that were covered in the some
of the previous sessions, but now we can see in detail.

### Listening to Events Emitted by a Smart Contract

  * [Deck][25]
  * [Hands-on][28]

Our final hands-on exercise was to interact with our [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s not
in the request-response variety, but rather in the listening for events
variety. Web3.js makes this very easy to do, and we set up a listener
that prints out event details whenever the ones we were interested in
did something.

We wanted to get further by also updating the web page to list details,
but that needed to be skipped in light of time - we always run out of it
in our final exercise in each session.

There were further tasks around filtering events that were left as take-
home tasks for all of you.

## Thanks

Thanks to [Lifelong Learning Institute (SkillsFutureSG)][29] for
sponsoring us via their learning circles program - you have them to
thank for the F&B.

Thanks to [Chainstack][30] for hosting us at their excellent space.
Thanks Ashlie & Dennis for helping us run the event, and helping with
the set up.

## Next session

RSVPs are now open - please let us know if you're attending, as it helps
us plan for seating, ordering F&B, etc:

[**RSVP** on eventbrite][31]

ðŸ¤˜ðŸ¤˜ðŸ¤˜

* * *

[][32]

* * *

#### Tags

  * [irl][33]
  * [s01][34]
  * [s01e06][35]
  * [summary][36]
  * [javascript][37]
  * [frontend][38]
  * [webpack][39]
  * [web3js][40]

   [1]: /img/dadc-logo.png
   [2]: / (Logo)
   [3]: /sessions
   [4]: /partners
   [5]: /projects
   [6]: /certificates
   [7]: data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIiB2ZXJzaW9uPSIxLjEiIGlkPSJDYXBhXzEiIHg9IjBweCIgeT0iMHB4IiB3aWR0aD0iNDM4LjU0OXB4IiBoZWlnaHQ9IjQzOC41NDlweCIgdmlld0JveD0iMCAwIDQzOC41NDkgNDM4LjU0OSIgc3R5bGU9ImVuYWJsZS1iYWNrZ3JvdW5kOm5ldyAwIDAgNDM4LjU0OSA0MzguNTQ5OyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI+CjxnPgoJPHBhdGggZD0iTTQwOS4xMzIsMTE0LjU3M2MtMTkuNjA4LTMzLjU5Ni00Ni4yMDUtNjAuMTk0LTc5Ljc5OC03OS44QzI5NS43MzYsMTUuMTY2LDI1OS4wNTcsNS4zNjUsMjE5LjI3MSw1LjM2NSAgIGMtMzkuNzgxLDAtNzYuNDcyLDkuODA0LTExMC4wNjMsMjkuNDA4Yy0zMy41OTYsMTkuNjA1LTYwLjE5Miw0Ni4yMDQtNzkuOCw3OS44QzkuODAzLDE0OC4xNjgsMCwxODQuODU0LDAsMjI0LjYzICAgYzAsNDcuNzgsMTMuOTQsOTAuNzQ1LDQxLjgyNywxMjguOTA2YzI3Ljg4NCwzOC4xNjQsNjMuOTA2LDY0LjU3MiwxMDguMDYzLDc5LjIyN2M1LjE0LDAuOTU0LDguOTQ1LDAuMjgzLDExLjQxOS0xLjk5NiAgIGMyLjQ3NS0yLjI4MiwzLjcxMS01LjE0LDMuNzExLTguNTYyYzAtMC41NzEtMC4wNDktNS43MDgtMC4xNDQtMTUuNDE3Yy0wLjA5OC05LjcwOS0wLjE0NC0xOC4xNzktMC4xNDQtMjUuNDA2bC02LjU2NywxLjEzNiAgIGMtNC4xODcsMC43NjctOS40NjksMS4wOTItMTUuODQ2LDFjLTYuMzc0LTAuMDg5LTEyLjk5MS0wLjc1Ny0xOS44NDItMS45OTljLTYuODU0LTEuMjMxLTEzLjIyOS00LjA4Ni0xOS4xMy04LjU1OSAgIGMtNS44OTgtNC40NzMtMTAuMDg1LTEwLjMyOC0xMi41Ni0xNy41NTZsLTIuODU1LTYuNTdjLTEuOTAzLTQuMzc0LTQuODk5LTkuMjMzLTguOTkyLTE0LjU1OSAgIGMtNC4wOTMtNS4zMzEtOC4yMzItOC45NDUtMTIuNDE5LTEwLjg0OGwtMS45OTktMS40MzFjLTEuMzMyLTAuOTUxLTIuNTY4LTIuMDk4LTMuNzExLTMuNDI5Yy0xLjE0Mi0xLjMzMS0xLjk5Ny0yLjY2My0yLjU2OC0zLjk5NyAgIGMtMC41NzItMS4zMzUtMC4wOTgtMi40MywxLjQyNy0zLjI4OWMxLjUyNS0wLjg1OSw0LjI4MS0xLjI3Niw4LjI4LTEuMjc2bDUuNzA4LDAuODUzYzMuODA3LDAuNzYzLDguNTE2LDMuMDQyLDE0LjEzMyw2Ljg1MSAgIGM1LjYxNCwzLjgwNiwxMC4yMjksOC43NTQsMTMuODQ2LDE0Ljg0MmM0LjM4LDcuODA2LDkuNjU3LDEzLjc1NCwxNS44NDYsMTcuODQ3YzYuMTg0LDQuMDkzLDEyLjQxOSw2LjEzNiwxOC42OTksNi4xMzYgICBjNi4yOCwwLDExLjcwNC0wLjQ3NiwxNi4yNzQtMS40MjNjNC41NjUtMC45NTIsOC44NDgtMi4zODMsMTIuODQ3LTQuMjg1YzEuNzEzLTEyLjc1OCw2LjM3Ny0yMi41NTksMTMuOTg4LTI5LjQxICAgYy0xMC44NDgtMS4xNC0yMC42MDEtMi44NTctMjkuMjY0LTUuMTRjLTguNjU4LTIuMjg2LTE3LjYwNS01Ljk5Ni0yNi44MzUtMTEuMTRjLTkuMjM1LTUuMTM3LTE2Ljg5Ni0xMS41MTYtMjIuOTg1LTE5LjEyNiAgIGMtNi4wOS03LjYxNC0xMS4wODgtMTcuNjEtMTQuOTg3LTI5Ljk3OWMtMy45MDEtMTIuMzc0LTUuODUyLTI2LjY0OC01Ljg1Mi00Mi44MjZjMC0yMy4wMzUsNy41Mi00Mi42MzcsMjIuNTU3LTU4LjgxNyAgIGMtNy4wNDQtMTcuMzE4LTYuMzc5LTM2LjczMiwxLjk5Ny01OC4yNGM1LjUyLTEuNzE1LDEzLjcwNi0wLjQyOCwyNC41NTQsMy44NTNjMTAuODUsNC4yODMsMTguNzk0LDcuOTUyLDIzLjg0LDEwLjk5NCAgIGM1LjA0NiwzLjA0MSw5LjA4OSw1LjYxOCwxMi4xMzUsNy43MDhjMTcuNzA1LTQuOTQ3LDM1Ljk3Ni03LjQyMSw1NC44MTgtNy40MjFzMzcuMTE3LDIuNDc0LDU0LjgyMyw3LjQyMWwxMC44NDktNi44NDkgICBjNy40MTktNC41NywxNi4xOC04Ljc1OCwyNi4yNjItMTIuNTY1YzEwLjA4OC0zLjgwNSwxNy44MDItNC44NTMsMjMuMTM0LTMuMTM4YzguNTYyLDIxLjUwOSw5LjMyNSw0MC45MjIsMi4yNzksNTguMjQgICBjMTUuMDM2LDE2LjE4LDIyLjU1OSwzNS43ODcsMjIuNTU5LDU4LjgxN2MwLDE2LjE3OC0xLjk1OCwzMC40OTctNS44NTMsNDIuOTY2Yy0zLjksMTIuNDcxLTguOTQxLDIyLjQ1Ny0xNS4xMjUsMjkuOTc5ICAgYy02LjE5MSw3LjUyMS0xMy45MDEsMTMuODUtMjMuMTMxLDE4Ljk4NmMtOS4yMzIsNS4xNC0xOC4xODIsOC44NS0yNi44NCwxMS4xMzZjLTguNjYyLDIuMjg2LTE4LjQxNSw0LjAwNC0yOS4yNjMsNS4xNDYgICBjOS44OTQsOC41NjIsMTQuODQyLDIyLjA3NywxNC44NDIsNDAuNTM5djYwLjIzN2MwLDMuNDIyLDEuMTksNi4yNzksMy41NzIsOC41NjJjMi4zNzksMi4yNzksNi4xMzYsMi45NSwxMS4yNzYsMS45OTUgICBjNDQuMTYzLTE0LjY1Myw4MC4xODUtNDEuMDYyLDEwOC4wNjgtNzkuMjI2YzI3Ljg4LTM4LjE2MSw0MS44MjUtODEuMTI2LDQxLjgyNS0xMjguOTA2ICAgQzQzOC41MzYsMTg0Ljg1MSw0MjguNzI4LDE0OC4xNjgsNDA5LjEzMiwxMTQuNTczeiIvPgo8L2c+CjxkaXYgeG1sbnM9IiIgaWQ9ImRpdlNjcmlwdHNVc2VkIiBzdHlsZT0iZGlzcGxheTogbm9uZSIvPjxzY3JpcHQgeG1sbnM9IiIgaWQ9Imdsb2JhbFZhcnNEZXRlY3Rpb24iIHNyYz0iY2hyb21lLWV4dGVuc2lvbjovL2Nta2RibWZuZGtmZ2VibGRobmtiZmhsbmVlZmRhYWlwL2pzL3dyc19lbnYuanMiLz48L3N2Zz4K
   [8]: https://github.com/dapps-dev-club
   [9]: data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNDUgMjQwIj48cGF0aCBkPSJNMTA0LjQgMTAzLjljLTUuNyAwLTEwLjIgNS0xMC4yIDExLjFzNC42IDExLjEgMTAuMiAxMS4xYzUuNyAwIDEwLjItNSAxMC4yLTExLjEuMS02LjEtNC41LTExLjEtMTAuMi0xMS4xek0xNDAuOSAxMDMuOWMtNS43IDAtMTAuMiA1LTEwLjIgMTEuMXM0LjYgMTEuMSAxMC4yIDExLjFjNS43IDAgMTAuMi01IDEwLjItMTEuMXMtNC41LTExLjEtMTAuMi0xMS4xeiIvPjxwYXRoIGQ9Ik0xODkuNSAyMGgtMTM0QzQ0LjIgMjAgMzUgMjkuMiAzNSA0MC42djEzNS4yYzAgMTEuNCA5LjIgMjAuNiAyMC41IDIwLjZoMTEzLjRsLTUuMy0xOC41IDEyLjggMTEuOSAxMi4xIDExLjIgMjEuNSAxOVY0MC42YzAtMTEuNC05LjItMjAuNi0yMC41LTIwLjZ6bS0zOC42IDEzMC42cy0zLjYtNC4zLTYuNi04LjFjMTMuMS0zLjcgMTguMS0xMS45IDE4LjEtMTEuOS00LjEgMi43LTggNC42LTExLjUgNS45LTUgMi4xLTkuOCAzLjUtMTQuNSA0LjMtOS42IDEuOC0xOC40IDEuMy0yNS45LS4xLTUuNy0xLjEtMTAuNi0yLjctMTQuNy00LjMtMi4zLS45LTQuOC0yLTcuMy0zLjQtLjMtLjItLjYtLjMtLjktLjUtLjItLjEtLjMtLjItLjQtLjMtMS44LTEtMi44LTEuNy0yLjgtMS43czQuOCA4IDE3LjUgMTEuOGMtMyAzLjgtNi43IDguMy02LjcgOC4zLTIyLjEtLjctMzAuNS0xNS4yLTMwLjUtMTUuMiAwLTMyLjIgMTQuNC01OC4zIDE0LjQtNTguMyAxNC40LTEwLjggMjguMS0xMC41IDI4LjEtMTAuNWwxIDEuMmMtMTggNS4yLTI2LjMgMTMuMS0yNi4zIDEzLjFzMi4yLTEuMiA1LjktMi45YzEwLjctNC43IDE5LjItNiAyMi43LTYuMy42LS4xIDEuMS0uMiAxLjctLjIgNi4xLS44IDEzLTEgMjAuMi0uMiA5LjUgMS4xIDE5LjcgMy45IDMwLjEgOS42IDAgMC03LjktNy41LTI0LjktMTIuN2wxLjQtMS42czEzLjctLjMgMjguMSAxMC41YzAgMCAxNC40IDI2LjEgMTQuNCA1OC4zIDAgMC04LjUgMTQuNS0zMC42IDE1LjJ6Ii8+PC9zdmc+
   [10]: https://discordapp.com/invite/eM9Vv7P
   [11]: data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij48cGF0aCBkPSJNMCAwdjI0aDI0di0yNGgtMjR6bTYuMTY4IDIwYy0xLjE5NyAwLTIuMTY4LS45NjktMi4xNjgtMi4xNjVzLjk3MS0yLjE2NSAyLjE2OC0yLjE2NSAyLjE2Ny45NjkgMi4xNjcgMi4xNjUtLjk3IDIuMTY1LTIuMTY3IDIuMTY1em01LjE4IDBjLS4wNDEtNC4wMjktMy4zMTQtNy4yOTgtNy4zNDgtNy4zMzl2LTMuMjA3YzUuODE0LjA0MSAxMC41MTggNC43MzkgMTAuNTYgMTAuNTQ2aC0zLjIxMnptNS40NDEgMGMtLjAyMS03LjA2My01LjczNi0xMi43NjEtMTIuNzg5LTEyLjc5MnYtMy4yMDhjOC44My4wMzEgMTUuOTggNy4xNzkgMTYgMTZoLTMuMjExeiIvPjwvc3ZnPg==
   [12]: /rss.xml
   [13]: data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAECAYAAACOXx+WAAAACXBIWXMAAAsSAAALEgHS3X78AAABNklEQVQY02PYsW+H2LqtKyP2HNymzwAE////ZwNidiDmffX2jTKIDRLftGOj59TZE6OXrVro/ejZA+OjR/dZLVg4r2D+0qUxUH1MIMwwb9nClHnL5v1fumZpT0NtfUVoWPzblOS0V+1tHS8Lisr+B4fGvI5LzttfUlX+NSEj5X9bb9v/OYvm/c0tLvhTWFb+PzEp93dZZcXJlraWWzkltbcZpsxe5OgblfzfydNjZUVN22TfmPz/nv6JD0pKqk6lpmXtDguLe11QUPo/LiX1t7G1/X9dU6P/JaUlP7Nz8v7HxCX/b8ou+VpcUvIoPjHlVkp6zjWGhRt2CQRmNYQmZpdq7bvwjhXqXWYGKAAFwdtn9xXnL11oH5OSHmTj5By9ZOGcqA1LZhWtXDLP6/TpfYpANYww9QApkafGej7kfgAAAABJRU5ErkJggg==
   [14]: /static/57ad772a2a1158b23b8e348262f9d2aa/e119a/dadc-s01e06-roundup.png
   [15]: /2019-05-17-dapps-dev-club-6th-session-videos/ (Web3 - Videos from S01E06 of DApps Dev Club)
   [16]: https://i.giphy.com/media/coYo4nM8jE1TW/giphy.webp
   [17]: https://www.linkedin.com/in/geraldnahhawyuan/
   [18]: https://www.linkedin.com/in/jack-ng-b2593b151
   [19]: https://www.linkedin.com/in/arif-rahman-86785a136/
   [20]: https://docs.microsoft.com/en-us/powershell/
   [21]: https://docs.microsoft.com/en-us/windows/wsl/install-win10
   [22]: https://dappsdev.org/deck/s01e06/#setup
   [23]: /hands-on/web3/project-setup/
   [24]: /hands-on/web3/scaffold/
   [25]: https://dappsdev.org/deck/s01e06/#interactions
   [26]: /hands-on/web3/query-state/
   [27]: /hands-on/web3/mutate-state/
   [28]: /hands-on/web3/listen-events/
   [29]: https://www.lli.sg/
   [30]: https://chainstack.com/
   [31]: https://dappsdev-s01e07.eventbrite.com/
   [32]: https://dappsdev.org/blog/2019-05-16-dapps-dev-club-6th-session-roundup/
   [33]: /tags/irl/
   [34]: /tags/s-01/
   [35]: /tags/s-01-e-06/
   [36]: /tags/summary/
   [37]: /tags/javascript/
   [38]: /tags/frontend/
   [39]: /tags/webpack/
   [40]: /tags/web-3-js/