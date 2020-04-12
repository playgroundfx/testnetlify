+++
categories = ["Cryptocurrency", "Blockchain", "SmartContract"]
date = "2019-03-14"
description = "Round up of session #02"
tags = ["Cryptocurrency", "Blockchain", "SmartContract"]
title = "Round up of session #02"
type = "post"
+++

[![DApps Dev Club][1]][2]

[Sessions][3][Partners][4][Projects][5][Certificates][6]

[![Github][7]][8][![Discord][9]][10][![RSS Feed][11]][12]

# Round up of session #02

![][13]![][14]

 _2nd session - Tech overview - EVM + Smart Contracts + Web3_

DApps Dev Club held its second session - Technical overview - on
Tuesday, where we covered the Ethereum Virtual Machine, Smart Contracts,
and Web3.

Each of these three things are hard to explain without first knowing what the other two of them are, so the over-arching idea was to go cover each of these briefly, in a single session, before we delve into the details about them in subsequent sessions. Hence we had an "overview". We could call this, to borrow a very apt computer science terminology, a [_breadth-first_ approach][15] (with our subsequent sessions being [_depth-first_][16]).

Hopefully all who attended came away with an understanding of not only
what the purpose of each of these three things are, but also how they
they _integrate_ , and fit in with each other.

## Format

As promised in the [kickoff session][17], this session saw a small, but
deliberate, shift from being a one-way information presentation session
- akin to a lecture - and towards an interactive, hands-on session -
akin to a **workshop**. While we did spend most of the time looking at
information on slides, we also spent a some time exploring and trying
out mini-exercises on your computers.

The other changes that happened naturally, was that the talking was a
lot more bi-directional, with you fielding many questions and comments.

We hope that this continues, being more **participatory** \- with both
working hands-on on something, as well as with discussion - as that is
the core or essence of being a **technical book club**!

As with the kickoff session, we recorded this one too. ~~, and will post
them as soon as we can!~~

[Videos for Session #02][18] are now up.

## Deck

If you would like to review the slide deck that was presented again, or
follow along while watching the recordings, or get at a hyperlink that
we mentioned - [here it is!][19]

## Hands on

We had two hands-on parts during the session.

### Compile solidity in Remix

This exercise was one to simply get our feet wet:

  * Open up Remix
  * Copy-and-paste a sample Solidity file into it
  * Press the compile button
  * Inspect the compiler output
  * Relate this compiler output to EVM byte codes and op codes that were just discussed

Here are [instructions we used][20], if you would like to follow along.

### Code state [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)

In the kickoff session, we explained what a blockhain was using Anders'
Blockchain demo. This demo was great because it starts from the most
primitive feature, the hash, and then builds up, step-by-step, to
showing how a [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/) works.

However, towards the end, it becomes specific to transfers of currency,
which is merely one of the use cases for a [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/). In Ethereum (as
with many others since it), there is also **code and state** , the
building blocks that enable [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s.

So we [forked Anders' Blockchain demo][21] to add a new tab that adds a
demonstration for precisely that - code and state on a [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/).

Here are the [instructions to follow along][22].

## Questions

There were quite a few questions that were fielded.

A few of them were related to the nonce in a block:

  * Do nodes share/ publish their nonces?
  * Why is the nonce included in the data that is hashed?

A few of them were related to the mechanics of Nakamoto consensus:

  * How does a soft fork arise?
  * How about hash collisions?

Finally, a few questions about the Ethereum network:

  * How many nodes are currently on the Ethereum main net?
  * Is the price of gas stable, or does it fluctuate?

Hopefully these questions were answered well!

## Favourites

The code state [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/) demo was a hit, with lots of **Aha** moments
all around. We even got requests to _take it further_ , by making it a
[smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/) [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/) demo!

The other thing that perhaps wasn't so much a favourite, as it was
something that provoked a very obvious reaction (gasps!) was the cost of
storage. One participant even remarked during the break that she was now
reconsidering about whether something that she had in mind could be
feasibly built on a [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/).

## Thanks

A huge thanks to [Chainstack][23] and [Acronis][24] for hosting us at
their excellent office space. Especially Ashlie for organising the event
space, and Dennis for supporting the AV set up.

Thanks to [Spartan][25] for sponsoring the refreshments, and their
community outreach.

Thanks to [StartupToken][26] for their community outreach.

Thanks also to Wing & Gerald for their on-site assistance in running the
event.

## Next session

Our third session will be on Tuesday 26th March. Please let us know if
you're planning to attend, as it helps us to plan for seating, et
cetera.

[RSVP on eventbrite][27]

* * *

[][28]

* * *

#### Tags

  * [irl][29]
  * [s01][30]
  * [s01e02][31]
  * [summary][32]
  * [evm][33]
  * [[smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)][34]
  * [web3][35]

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
   [13]: data:image/jpeg;base64,/9j/2wBDABALDA4MChAODQ4SERATGCgaGBYWGDEjJR0oOjM9PDkzODdASFxOQERXRTc4UG1RV19iZ2hnPk1xeXBkeFxlZ2P/2wBDARESEhgVGC8aGi9jQjhCY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2P/wgARCAANABQDASIAAhEBAxEB/8QAGAAAAwEBAAAAAAAAAAAAAAAAAAMFAgT/xAAUAQEAAAAAAAAAAAAAAAAAAAAA/9oADAMBAAIQAxAAAAHtm2kjjYf/xAAZEAADAQEBAAAAAAAAAAAAAAABAgMAEhP/2gAIAQEAAQUCvYSX2pQovC8jTgkzv//EABQRAQAAAAAAAAAAAAAAAAAAABD/2gAIAQMBAT8BP//EABQRAQAAAAAAAAAAAAAAAAAAABD/2gAIAQIBAT8BP//EAB4QAAIBAwUAAAAAAAAAAAAAAAABMREhIgIQEhNh/9oACAEBAAY/ApyOvksvCiHaZK6Vfb//xAAbEAEAAwEAAwAAAAAAAAAAAAABAFFhIRAxgf/aAAgBAQABPyFRxQrWASTPYQPoOsXClKvcRlLZ4//aAAwDAQACAAMAAAAQN9//xAAUEQEAAAAAAAAAAAAAAAAAAAAQ/9oACAEDAQE/ED//xAAUEQEAAAAAAAAAAAAAAAAAAAAQ/9oACAECAQE/ED//xAAeEAEAAgIBBQAAAAAAAAAAAAABESEAMVFBYXGhsf/aAAgBAQABPxAvkZULBeho+5NRRc2woaaNOFpyVRbS1e64PaoD7OcSFF0VOBLWAhbL4z//2Q==
   [14]: /static/5898aca6b469e98b49c399ec8cbb55f0/3df8f/dadc-s01-e02-featured-image.jpeg
   [15]: https://en.wikipedia.org/wiki/Breadth-first_search
   [16]: https://en.wikipedia.org/wiki/Depth-first_search
   [17]: https://dappsdev.org/blog/2018-02-25-dapps-dev-club-kickoff-session/
   [18]: /blog/2019-03-16-dapps-dev-club-2nd-session-videos/
   [19]: https://dappsdev.org/deck/s01e02/ (DApps Dev Club S01E02 Slide Deck)
   [20]: https://gist.github.com/bguiz/3d7048362323cc76931f72719972dc3b (compile and inspect solidity demo instructions)
   [21]: https://github.com/anders94/[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)-demo/compare/master...dapps-dev-club:feat/codestate
   [22]: https://gist.github.com/bguiz/d9737ab76bf58ab20b4884f3f15bcb39 (code state [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/) demo instructions)
   [23]: https://chainstack.com
   [24]: https://www.acronis.com/
   [25]: https://spartangroup.io
   [26]: https://www.startuptoken.com
   [27]: https://dappsdev-s01e03.eventbrite.com/
   [28]: https://dappsdev.org/blog/2019-03-14-dapps-dev-club-2nd-session-roundup/
   [29]: /tags/irl/
   [30]: /tags/s-01/
   [31]: /tags/s-01-e-02/
   [32]: /tags/summary/
   [33]: /tags/evm/
   [34]: /tags/smart-contract/
   [35]: /tags/web-3/