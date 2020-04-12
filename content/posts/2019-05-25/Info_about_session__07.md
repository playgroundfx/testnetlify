+++
categories = ["Cryptocurrency", "Blockchain", "SmartContract"]
date = "2019-05-25"
description = "Info about session #07"
tags = ["Cryptocurrency", "Blockchain", "SmartContract"]
title = "Info about session #07"
type = "post"
+++

[![DApps Dev Club][1]][2]

[Sessions][3][Partners][4][Projects][5][Certificates][6]

[![Github][7]][8][![Discord][9]][10][![RSS Feed][11]][12]

# Info about session #07

![][13]![][14]

 _What you need to know about our 7th session!_

DApps Dev Club is holding its 7th session, about [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)
security, on Tuesday, 28th May.

[**RSVP now!**][15]

Here's what you need to know!

## Event

The session will be held at [BitTemple's][16] office in Raffles Place.

Thanks Solomon for helping us run the event!

## Topics

In our previous session, we wrote the client that allows an end user to
interact with our [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s, using a combination of various front-
end web development tools, together with web3.js.

In session #04 we wrote a [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/), and in session #05, we wrote
tests against our [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s. In this session, we will learn about
[smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/) security, which relates more to what we did in sessions
#04 and #05, and does **not** exactly flow on from the previous session.
So if you need a recap, please read the summary posts, or watch the
videos recorded, for those sessions if you would like a refresher:

  * [Session #04 summary][17]
  * [Session #04 videos][18]
  * [Session #05 summary][19]
  * [Session #05 videos][20]

Specifically, for this session, what we have lined up:

  * Demonstration of a common security vulnerability: Reentrance

    * We will write a vulnerable contract, then write another contract that successfully attacks it, and finally fix the contract such that it cannot be attacked using the same method.
  * Introduce security training games, and play them a little bit
  * Look at various Solidity developer tools that aid in the development of [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s.

    * Focus on tools that performs static and dynamic analyses.

As with the previous session, there will be hands-on parts. However, as
mentioned in the **Reflections** section of the [session #06 summary
post][21], we will be kicking the difficulty level of this session
**down a notch** , so that it will be easier to follow along. If you
enjoyed the pace and complexity of sessions #03 and #04, you'll enjoy
this session too! ðŸ˜�

Security is a **huge** topic within [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s, and a single
session on it would not everbe sufficient to cover it in any reasonable
amount of detail. In fact, security alone could be the basis of an
entire series of sessions! Thus, this session has been designed as more
of an introductory level **survey** of the various facets of smart
contract security, with the intended take away for attendees being that
you are **aware** of them, and are eqiuipped with the resources to delve
deeper into them when the need strikes.

## Preparation

In this session, most of the things that we will be doing are browser
based, and to follow along you will need Chrome or Chromium, with
[MetaMask][22] installed as a browser plugin.

In order to follow along with the secruity training games, you will need
some **Ropsten test net Ether** , so please find a faucet and grab some
Ether ahead of the session, so that you do not need to waste time during
the session.

Further to this, if you would like to follow along and try out the demos
as well, you should also install the following:

  * [slither][23] \- `pip install slither-analyzer`

    * Note that you will need a Python 3 environment set up for this to work, which contradicts the requirement for `node-gyp` with Python 2 ðŸ˜¬ so this might make make it difficult to install.
  * [solidity-coverage][24] \- `npm i -g solidity-coverage`

    * This should be an easy installation, if you have prweviously installed truffle successfully.
  * If you do not want to use Ropsten, you have the option of running things locally:

    * Clone the [ethernaut][25] git repo, and follow the instructions for `localhost` in the readme.
    * Note that the installation for this is quite time consuming, be warned!
  * If you would like to use the newer, snazzier, edition of Remix IDE that has just been released, you can run that locally too:

    * get [remix-ide][26] \- `npm i -g remix-ide`
    * This should be quite an easy installation as well, if you have previously intsalled truffle.

Do _attempt_ to get these installed prior to the session if you can - as
it will be fun to follow along with - but no worries if you cannot, as
there will be live demos of these anyway! The only true requirements
here are Chrome + MetaMask.

## Projects

In the previous session, a few of you did say that you felt you were
ready to start developing your own DApps, and asked for some project
ideas to work on. We're stoked!

a€¦ for those who are interested, please take your ideas to our [chat
group][15], or come and talk with us during the session - we have a few
interesting ones for you to tackle!

## Next session

[**RSVP** on eventbrite][15]

a€¦ it helps us plan for seating, ordering F&B, et cetera.

See you all again soon!

* * *

[][27]

* * *

#### Tags

  * [irl][28]
  * [s01][29]
  * [s01e07][30]
  * [security][31]
  * [audit][32]
  * [lint][33]
  * [coverage][34]
  * [static analysis][35]

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
   [13]: data:image/jpeg;base64,/9j/2wBDABALDA4MChAODQ4SERATGCgaGBYWGDEjJR0oOjM9PDkzODdASFxOQERXRTc4UG1RV19iZ2hnPk1xeXBkeFxlZ2P/2wBDARESEhgVGC8aGi9jQjhCY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2P/wgARCAAKABQDASIAAhEBAxEB/8QAFgABAQEAAAAAAAAAAAAAAAAAAAUC/8QAFAEBAAAAAAAAAAAAAAAAAAAAAP/aAAwDAQACEAMQAAABoza40D//xAAZEAACAwEAAAAAAAAAAAAAAAAAAgEDEUH/2gAIAQEAAQUCtl8pV3Yk6f/EABQRAQAAAAAAAAAAAAAAAAAAABD/2gAIAQMBAT8BP//EABQRAQAAAAAAAAAAAAAAAAAAABD/2gAIAQIBAT8BP//EABsQAAEEAwAAAAAAAAAAAAAAABIAASAhIiNh/9oACAEBAAY/AsGtbCHsf//EABoQAQACAwEAAAAAAAAAAAAAAAEAERAxQSH/2gAIAQEAAT8hAy9m1oJR6j6j245lHGP/2gAMAwEAAgADAAAAEHff/8QAFBEBAAAAAAAAAAAAAAAAAAAAEP/aAAgBAwEBPxA//8QAFBEBAAAAAAAAAAAAAAAAAAAAEP/aAAgBAgEBPxA//8QAHRAAAgEEAwAAAAAAAAAAAAAAAREhABAxcUFRYf/aAAgBAQABPxB56UBodnylcxa40pkiS1YQQwBk51THIOONW//Z
   [14]: /static/2408d65933c8457f57aec11e58752e89/3df8f/dadc-s01e07-featured-image.jpeg
   [15]: https://dappsdev-s01e07.eventbrite.com/
   [16]: https://bittemple.io/
   [17]: /blog/2019-04-12-dapps-dev-club-4th-session-roundup/
   [18]: /blog/2019-04-13-dapps-dev-club-4th-session-videos/
   [19]: /blog/2019-05-02-dapps-dev-club-5th-session-roundup/
   [20]: /blog/2019-05-01-dapps-dev-club-5th-session-videos/
   [21]: /blog/2019-05-16-dapps-dev-club-6th-session-roundup/
   [22]: https://metamask.io/
   [23]: https://github.com/crytic/slither
   [24]: https://github.com/sc-forks/solidity-coverage
   [25]: https://github.com/OpenZeppelin/ethernaut
   [26]: https://github.com/[Ethereum](https://www.playgroundfx.com/blog/the-creator-of-ethereum/)/remix-ide
   [27]: https://dappsdev.org/blog/2019-05-25-dapps-dev-club-7th-session-info/
   [28]: /tags/irl/
   [29]: /tags/s-01/
   [30]: /tags/s-01-e-07/
   [31]: /tags/security/
   [32]: /tags/audit/
   [33]: /tags/lint/
   [34]: /tags/coverage/
   [35]: /tags/static-analysis/