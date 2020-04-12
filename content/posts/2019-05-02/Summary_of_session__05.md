+++
categories = ["Cryptocurrency", "Blockchain", "SmartContract"]
date = "2019-05-02"
description = "Summary of session #05"
tags = ["Cryptocurrency", "Blockchain", "SmartContract"]
title = "Summary of session #05"
type = "post"
+++

[![DApps Dev Club][1]][2]

[Sessions][3][Partners][4][Projects][5][Certificates][6]

[![Github][7]][8][![Discord][9]][10][![RSS Feed][11]][12]

# Summary of session #05

![][13]![][14]

 _Testing: Mocha + truffle test + data storage + state machines + events
+ (mocking)_

The DApps Dev Club held its fifth session, about testing smart
contracts, a couple of days ago, on Tuesday evening at BitTemple.

We spent some time covering software testing in general, and capped that
off with an introduction to testing vanilla Javascript using **Mocha**
as a test runner. Subsequently, we built upon that by using **truffle
test** to test [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s in Solidity.

Our videos are already up, and our [video post for this session][15] has
you covered!

## Rescheduling

This session was originally scheduled to run on Tuesday 23rd April 2019,
but BitTemple needed to reschedule us. We tried our best to find an
alternative venue on the same date. Securing a venue for a tech meetup
is extremely difficult - let alone securing one at short notice - and
our efforts were in vain.

So we held our session exactly one week later on Tuesday 30th April
2019, instead. Apologies to everyone who was inconvenienced, we wish
that we had more within the locus of our control. For those of you who
had RSVP'ed for the original date, but were not able to make it to the
rescheduled date, hopefully you're able to catch up by watching [the
videos][15]!

## Format

Continuing with the bar set in the previous session, this one was almost
entirely comprised of hands-on stuff, and very little theory from a
slide deck.

Fun fact **#1** : In session #05 we broke the record for number of
hands-on parts attempted - but we did not manage to get through the
final one, so &hellip ðŸ¤*.

Fun fact **#2** : This session was also the first time there was a
blunder in a live demo. As the stuff that we are dealing with gets more
complex, this is probably going to happen more frequently. Frankly I'm
pleasantly surprised that we have managed to get through as many
sessions without one as we have - the demo gods have indeed been kind to
me so far! ðŸ˜‡

## Difficulty and pace

In previous sessions, some of you have given us feedback that the pace
was either too fast or too slow. We've taken that on board and
experimented a little. This time for each of the hands-on parts, we
included a little stretch goal, which was more or less:

"Do this task ___, but we're not telling you how, you need to figure it
out on your own. BTW, here are some hints: ___"

That seemed to work really well, because after the session, those of you
who talked to me all said that the pace was right. This is the first
time that that has happened in our sessions! ðŸŽ‰ðŸŽ‰ðŸŽ‰

## Above and beyond

A few of you who attend these sessions have really stepped up, going
from attending the sessions, to actively helping out.

Thanks [Kenneth Goh][16] for helping out during the session, and getting
people unstuck where they've gotten stuck.

Thanks [Jack Ng][17] for also helping out during the session, and
getting people unstuck. Also, for **reviewing** my hands-on materials
prior to the session, and giving me quite **detailed feedback** on it -
which was certainly put to good use!

You deserve a shout out for being awesome! ðŸ™ŒðŸ™Œ The session would
not have progressed as **smoothly** as it did without you!

## Topics

### Mocha

  * [Deck][18]
  * [Hands-on][19]

In our very first section, we ditched [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s, Solidity, and
decentralised application development entirely, and focused purely on
Javascript instead. The idea here was to lay the foundation for the next
sections.

The learning objectives here were threefold:

  * Testing and software engineering principles
  * Writing tests to be run by Mocha
  * Javascript (the language)

Let's summarise each of them next.

#### Testing and software engineering principles

We discussed the implementations, specifications, test runners, and the
relationship between the three.

We also discussed what I'm choosing to call the **implementation
specification correctness quadrants** :

[ ![Implementation specification correctness quadrants][20] ][21]

(you'll have to excuse my terrible graphic design skills - I clearly
have yet to get past the mspaint.exe level of ability)

#### Writing tests to be run by Mocha

Here we discussed the basics like the `describe` and `it` blocks, and
[how to](https://www.playgroundfx.com/blog/forex-trading-how-to/) use them. We also took a look at using `assert` (the NodeJs core
module) to write assertions within our tests.

We also did a brief detour, for those who were new to it, into using git
and github for version control of your project folder.

If you have followed along with the hands-on parts during our sessions,
or even in your own time, please commit, push, and add a link to your
project in [our chat group][22] \- it would be great to see some of the
stuff that we have all built together! ðŸ"¥ðŸ"¥ðŸ"¥

#### Javascript (the language)

This was more of an implicit goal rather than an implicit goal. When we
asked for a show of hands for who has written Javascript before, and
less than half of you present raised your hands. However, everyone was
able to follow along with the hands-on parts, so gentle on-ramping of
the language looks like it worked!

### Truffle testing set up

  * [Hands-on][23]

This section was a very brief interlude between going from using Mocha
to test vanilla Javascript files, to using truffle to test Solidity
[smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s.

The focus here was mainly pointing out the 1% extra features that
truffle test has that are built on top of Mocha.

### Data storage

  * [Deck][24]
  * [Hands-on][25]

When a [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/) is first deployed, it already has some initial
state. This is the easiest thing for one to possibly test in a smart
contract - in [terms](https://www.fintechee.com/terms/) of the complexity of the tests that need to be
written - so this is where we started!

Many of you, this was the **first time** that you have written a test
for a [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)! ðŸ'�ðŸ'�ðŸ'�

For some of you, it was the **first time** that you have written a test
for a [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/), **_and also_** the first time you have written a
test for **any type of code** at all! ðŸ'�ðŸ'�ðŸ'�ðŸ'�ðŸ'�

### State machines

  * [Deck][26]
  * [Hands-on][27]

We began this section with a short discussion on state machines, and
state transitions, int he context of [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s.

> A Scilla [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/) (and in general most [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s that you
see today) are stateful systems. This basically means that a smart
contract at any point of time can be said to be in a particular "state".
This "state" for instance can be a set of variables (and its current
value) or say map (in the case of ERC20 token contract) that stores
which user owns how many tokens. A state transition is a function that
allows users to change the state of the contract. For instance, the
transfer state transition function will allow users to transfer tokens
from one user to another and hence changing the map.

a€" Amrit Kumar

We took apart the quote above, by one of the creators of Scilla, the
programming language used to write [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s for a different
network, and discussed what it means, and what the implications are for
writing [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s in platforms such as the Ethereum Virtual
Machine.

Next, we did a hands-on where we wrote tests for state transitions.
There is a really interesting bit about the return values of Solidity
[functions](https://www.fintechee.com/tutorial-for-forex-trading/basic-functions/) which are state transitions (so go check it out).

As part of this hands-on, we also got to experiment with the **clean-
room environment** that the `contract` block from truffle test.

### Events

  * [Deck][28]
  * [Hands-on][29]

Here we discussed how events in Solidity map to logs in Ethereum, as
well as the distinction between "logs" and "structured logs".

In our hands-on we then wrote some tests for events.

We also introduce the `before` block from Mocha at this point.

### Mocking

  * [Deck][30]
  * [Hands-on][31]

At the beginning of this session, I said that most likely we will not
get through all of the material planned for the session, because we have
an audaciously large number of hands-on parts for this session. True
enough, that happened.

However, we managed to get through everything but the last hands-on. So
try this out for yourselves - all the material is available at the link
above! If you have any questions, or get stuck, et cetera, reach out at
[our chat group][32], or we might be able to discuss it at the beginning
of session #06.

## Thanks

Thanks to [Lifelong Learning Institute (SkillsFutureSG)][33] for
sponsoring us via their learning circles program - you have them to
thank for the F&B.

Thanks to [BitTemple][34] for hosting us at their excellent space.
Thanks Solomon for helping us run the event, and helping with the set
up.

## Next session

RSVPs are now open - please let us know if you're attending, as it helps
us plan for seating, ordering F&B, etc:

[**RSVP** on eventbrite][35]

ðŸ¤˜ðŸ¤˜ðŸ¤˜

* * *

[][36]

* * *

#### Tags

  * [irl][37]
  * [s01][38]
  * [s01e05][39]
  * [summary][40]
  * [solidity][41]
  * [mocha][42]
  * [testing][43]
  * [truffle][44]

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
   [13]: data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAECAYAAACOXx+WAAAACXBIWXMAAAsSAAALEgHS3X78AAABIUlEQVQY02P4//8/z/7NK/mBNPekCX2O2enJiRmZqSEzZ840ZQACoDgzEHMCMQcQszAgAZD44+cPRIA0G1xuUXfj56bc6B99lenfGgrS/7vZGv93sLH8HxcR+La9p2F3a0vTvdzkiI/tNdlvm2tKnrW3NR+rK8lZ1VpXvKeloe7jxO7W3zXFOa8XLZj7qCw79RhDXkz4l/QA568TylM/TW+t+NNVk/e/pbzgf2d13veswuBvGSlxd1Oig3ZNai7Zkp0Xd7EwL/19VWHOh8rinB9tlaWnp7c2LS3KjNubnZV+oyg94S3D/JWrRErKKoVmz1vJ+/T6ScNzB9b7bl46JWLPqrmO/1c/ZAd6BdmXDNdvbWR+/OYj/9uXL3kZ0ADI2wAdiaAEDb3Q4QAAAABJRU5ErkJggg==
   [14]: /static/7f8c7ca9fcc4317583c04762a65d0609/e119a/dadc-s01e05-roundup.png
   [15]: /blog/2019-05-01-dapps-dev-club-5th-session-videos/ (Videos from DApps Dev Club Session #05 on Testing)
   [16]: https://www.linkedin.com/in/kenneth-goh-65ba9525/
   [17]: https://www.linkedin.com/in/jack-ng-b2593b151
   [18]: https://dappsdev.org/deck/s01e05/#mocha
   [19]: /hands-on/mocha-intro/
   [20]: /static/0a23beca3cfbdf6bca79fac1818b23ec/bb194/implementation-specification-quadrants.png ()
   [21]: /static/0a23beca3cfbdf6bca79fac1818b23ec/bb194/implementation-specification-quadrants.png
   [22]: https://bit.co/dadc-chat (DApps Dev Club chat group)
   [23]: /hands-on/testing/truffle-setup/
   [24]: /deck/s01e05/#data-storage
   [25]: /hands-on/testing/solidity-data-storage/
   [26]: https://dappsdev.org/deck/s01e05/#state-machines
   [27]: /hands-on/testing/solidity-state-machines/
   [28]: /deck/s01e05/#events
   [29]: /hands-on/testing/solidity-events/
   [30]: /deck/s01e05/#mocking
   [31]: /hands-on/testing/solidity-mocks/
   [32]: https://bit.do/dadc-chat (The DApps Dev Club chat group)
   [33]: https://www.lli.sg/
   [34]: https://bittemple.io/
   [35]: https://dappsdev-s01e06.eventbrite.com/
   [36]: https://dappsdev.org/blog/2019-05-02-dapps-dev-club-5th-session-roundup/
   [37]: /tags/irl/
   [38]: /tags/s-01/
   [39]: /tags/s-01-e-05/
   [40]: /tags/summary/
   [41]: /tags/solidity/
   [42]: /tags/mocha/
   [43]: /tags/testing/
   [44]: /tags/truffle/