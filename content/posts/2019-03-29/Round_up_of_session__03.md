+++
categories = ["Cryptocurrency", "Blockchain", "SmartContract"]
date = "2019-03-29"
description = "Round up of session #03"
tags = ["Cryptocurrency", "Blockchain", "SmartContract"]
title = "Round up of session #03"
type = "post"
+++

[![DApps Dev Club][1]][2]

[Sessions][3][Partners][4][Projects][5][Certificates][6]

[![Github][7]][8][![Discord][9]][10][![RSS Feed][11]][12]

# Round up of session #03

![][13]![][14]

 _3rd session - Talking to Ethereum - EVM's Stack Based Execution +
Cryptographic Key Generation + MetaMask + Simple Transactions + DApp
Games_

DApps Dev Club held its third session - Talking to Ethereum - on
Tuesday, where the stack-based execution model used by the Ethereum
Virtual Machine, means to generate cryptographic keys for use in
Ethereum wallet software, using MetaMask, performing simple
transactions, and DApp Games.

We've _already_ posted [the videos from the session here][15].

The goal was originally to spend some time getting everyone set up to
use their networks to talk to the Ethereum network, followed by an
introduction to Solidity. However, we never fully got around to the
latter part, because we spent too long on the set up. We will cover this
in our next session instead!

## Format

As promised in the [kickoff session][16], and [session #02][17], we have
now finally transitioned from a one-way information transfer kind of
environment, akin to a lecturea€¦ to a more participatory hands-on kind
of environment, akin to a workshop.

Things are finally starting to feel like it is a **technical book club**
, as originally envisioned.

## Deck

If you would like to review the slide deck that was presented again, or
follow along while watching the recordings, or get at a hyperlink that
we mentioned - [here it is!][18]

## Topics

## EVM's stack-based execution model

The concept of a virtual machine as a software abstraction over hardware
execution was introduced in session #02, and along with it a brief
mention that Ethereum's virtual machine made use of a stack-based
execution model - but with no further details.

As we all will be learning about and making use of solidity compilers,
we thought it would best to visually show exactly what was meant by
that.

Using reverse-Polish-notation and EVM op codes we stepped through a
simple arithmetic operation with [illustrations for each step of the
way][19].

## Generating cryptographic keys Ethereum

In this section we talked about BIP39, BIP44, and BIP32, and how they
can be used to generate a large number of cryptographic keys from a
single seed phrase, in a secure way.

When talking about randomly generated entropy, [keep this XKCD comic in
mind][20]!

## Performing simple transactions

Next we installed MetaMask, which was introduced in session #02, this
time we made use of the seed phrase that we generated as an input, as
demonstrated that each _Account_ actually matches the keys generated
using BIP39.

Next, we used these accounts to send each other test-net Ethers, via
[this simple web page][21].

We also wrote random text strings onto the (test-net) [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/), just
for fun!

## Solidity

This is the section that we had been gearing up, never quite got enough
time. Instead we talked about a learning tool which teaches you [how to](https://www.playgroundfx.com/blog/forex-trading-how-to/)
build your own version of CryptoKitties - the DApp that was so popular
that it actually, at one point, "crashed" the Ethereum network with too
many transactions.

[CryptoZombies][22] is that game, except that instead of kittens, you
have Zombies.

## Reflections

**Pace** : Four of you said that the pace was too slow for you, during
the hands-on sections. We are trying to cater for everyone, but at the
same time feel your frustrations. But can we have our collective cake
and eat it too? Vedant came up with an interesting solution:

Have the ones who finish quicker go around the room and help the rest
who have not yet (completely optional, of course). This is totally in
the spirit of a technical book club, so let's try this out [our next
session][23], and see how it goes!

**Support** : We've received so much positive feedback with comments
such as:

> This has been something I've wanted to try out for a while, but never
got around to. I'm so glad that you're doing these sessions.

It is great that the stuff that we're doing in these sessions resonates
so well with you. Also we've noticed that there are a number of you who
have turned up at all three sessions so far - you're familiar faces
now!!

**Offering help** : We've also been getting offers from you as
participants to help us organising these sessions. From helping out with
the pre-session AV set up, to offering to help build demos for the
sessions. This is all great, and again, a very nice sign that we're
building a neat club here. Thank you everyone!

## Favourites

The favourite part about this session was the **simple transactions
hands-on**. For many of you, this would have been your first interaction
with the Ethereum network.

In addition to this, we sensed that quite a few of you were pretty
curious/ excited about being able to write not just transactional data,
but also completely arbitrary data, to an publicly available immutable
ledger.

One of the questions asked during the hands-on is also worth
highlighting here, which was:

> Why was there a fee to transfer zero Ether?

This was really interesting because it was a very concrete way to show
that executing a transaction is based solely on computational
complexity, and not a percentage based fee.

## Thanks

A huge thanks to [BitTemple][24] for hosting us at their excellent
office space. Especially Solomon for organising the event space.

Thanks also to Wing & Gerald for their on-site assistance in running the
event.

## Next session

Our fourth session will be on Tuesday 9th April. Please let us know if
you're planning to attend, as it helps us to plan!

[**RSVP** on eventbrite][23]

* * *

[][25]

* * *

#### Tags

  * [irl][26]
  * [s01][27]
  * [s01e03][28]
  * [summary][29]
  * [evm][30]
  * [rpn][31]
  * [cryptography][32]
  * [metamask][33]
  * [dapp][34]
  * [[Ethereum](https://www.playgroundfx.com/blog/the-creator-of-ethereum/)][35]

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
   [13]: data:image/jpeg;base64,/9j/2wBDABALDA4MChAODQ4SERATGCgaGBYWGDEjJR0oOjM9PDkzODdASFxOQERXRTc4UG1RV19iZ2hnPk1xeXBkeFxlZ2P/2wBDARESEhgVGC8aGi9jQjhCY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2P/wgARCAANABQDASIAAhEBAxEB/8QAGAAAAwEBAAAAAAAAAAAAAAAAAAMFAgT/xAAUAQEAAAAAAAAAAAAAAAAAAAAA/9oADAMBAAIQAxAAAAHtm2lDTYf/xAAZEAADAQEBAAAAAAAAAAAAAAABAgMAEhP/2gAIAQEAAQUCvYSX2pQovC8A5IJNt//EABQRAQAAAAAAAAAAAAAAAAAAABD/2gAIAQMBAT8BP//EABQRAQAAAAAAAAAAAAAAAAAAABD/2gAIAQIBAT8BP//EAB4QAAEDBAMAAAAAAAAAAAAAAAABETECEBIiEyFh/9oACAEBAAY/Ap2OPJNvBkF6mR6Ea3//xAAdEAEAAQQDAQAAAAAAAAAAAAABABEhMWEQQYFR/9oACAEBAAE/IVFj0Pm2ACTW8IHoO2IgimKmY8rD7x//2gAMAwEAAgADAAAAEAff/8QAFBEBAAAAAAAAAAAAAAAAAAAAEP/aAAgBAwEBPxA//8QAFBEBAAAAAAAAAAAAAAAAAAAAEP/aAAgBAgEBPxA//8QAHBABAAICAwEAAAAAAAAAAAAAAQARITFBUWGx/9oACAEBAAE/EC+xMQtF4NH2XcGZu2FDTg0wteWqLlMq+rGEdwGvTACgq3IOQXuBRV3P/9k=
   [14]: /static/5cabe6fcc898ab7888311531f7275559/3df8f/dadc-s01-e03-featured-image.jpeg
   [15]: /blog/2019-03-27-dapps-dev-club-3rd-session-videos/
   [16]: https://dappsdev.org/blog/2018-02-25-dapps-dev-club-kickoff-session/
   [17]: /blog/2019-03-14-dapps-dev-club-2nd-session-roundup/
   [18]: https://dappsdev.org/deck/s01e03/ (DApps Dev Club S01E03 Slide Deck)
   [19]: /deck/s01e03/#evm_stacks_steps
   [20]: https://xkcd.com/936/ (XKCD password strength)
   [21]: https://dappsdev.org/hands-on/simple-tx/
   [22]: https://cryptozombies.io/
   [23]: https://dappsdev-s01e04.eventbrite.com/
   [24]: https://bittemple.io/
   [25]: https://dappsdev.org/blog/2019-03-29-dapps-dev-club-3rd-session-roundup/
   [26]: /tags/irl/
   [27]: /tags/s-01/
   [28]: /tags/s-01-e-03/
   [29]: /tags/summary/
   [30]: /tags/evm/
   [31]: /tags/rpn/
   [32]: /tags/cryptography/
   [33]: /tags/metamask/
   [34]: /tags/dapp/
   [35]: /tags/[Ethereum](https://www.playgroundfx.com/blog/the-creator-of-ethereum/)/