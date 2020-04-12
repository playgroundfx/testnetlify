+++
categories = ["Cryptocurrency", "Blockchain", "SmartContract"]
date = "2019-02-25"
description = "Kickoff session | News | undefined"
tags = ["Cryptocurrency", "Blockchain", "SmartContract"]
title = "Kickoff session | News | undefined"
type = "post"
+++

[![DApps Dev Club][1]][2]

[Sessions][3][Partners][4][Projects][5][Certificates][6]

[![Github][7]][8][![Discord][9]][10][![RSS Feed][11]][12]

# Kickoff session

![][13]![][14]

 _Videos and summary of DApps Dev Club's first session_

Here is a round up of the _kickoff session_ of DApps Dev Club, which ran
last Wednesday (20th February 2019) at the Microsoft office in Marina
Boulevard.

The [slide deck][15] that was used during the session, has been
published, so now you can take a look.

**Highlights**

During the mid-session break, and after the session, we asked you what
your favourite parts were. Most of you said that your favourite part was
the live demo of the [Anders' Blockchain explainer][16] during the _Just
enough [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)_ segment - so a very quick recap of what we went
through:

  * _Hash_ : The three properties of a hash function that are useful in [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)s
  * _Block_ : Instead of arbitrary data, we're adding some structure to what is hashed
  * _Blockchain_ : Each block now contains the hash of the previous block, and how that relates to singly-linked lists
  * _Distributed [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)_ : Have three peers each create a block chain, but one of them maliciously creates a block with data different from the rest, and why the others choose to ignore it
  * We skipped: _Tokens_ and _Coinbase_ even though Ethereum has those too, we don't need to know that before we delve into DApps. You should totally explore that on your own though!

For some of the more advanced members in the audience, there are a
couple of things that were simplified or glossed over in the
demonstration. Thanks [Joey][17] for pointing these out to us.

  1. In the _distributed [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)_ section, multiple peers mined the same hash for the same block. In reality, peers can mine different hashes for the same block, by starting with different nonce values. Technically, the block contents are _almost_ identical, but not _exactly_ the same. The difference is the _nonce_. Since one of the properties of a hash function is that just a _slight change_ in the input causes the hash to be completely different, the blocks can have very different hashes.
  2. Also, in the _distributed [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)_ section, we used the [terms](https://www.fintechee.com/terms/) "real spend" and "double spend". The network cannot know whether any particular spend is a valid attempt, or a double spend attempt, without consensus first having taken place, and thus cannot have been known at this point. This was will become evident in the next section for _tokens_ , which was not demonstrated. Why not [try it out][18] yourself?

Another thing that you liked was the _Limitations_ part of the _What is
a DApp?_ segment. Going into further details on this was not within the
scope of the session; however, since there is interest, we will write up
a blog post focused on this topic. Watch this space!

**Videos**

We have got the _first two_ videos up already:

  * ðŸŽ¥ [Welcome][19]
  * ðŸŽ¥ [DApps Dev Club Introduction][20]

There are two more to come, for the _Just enough [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)_ , and the
_What is a DApp?_ segments - we will post another update when those are
ready!

This is our first time recording at a meetup - or recording anything
really - and we're pretty chuffed that we got it working at all! Sorry
about the extra low framerate from the camera trained on the speakers,
and the low volume audio. We will work on improving our recording skills
for the next session.

Also, a huge thanks to Michael Cheng of EngineersSG for producing this
wonderful [DIY tech meetup recording guide][21], and for answering a
slew of questions from us. Without his help, we would not have been able
to record our sessions!

**Reflections**

Based on the feedback that we have received from you so far, plus a
measure of contemplation:

  * More slides with pictures
  * Make demos more interactive
  * Improve on AV recording skills
  * Add QR codes for links in slides
  * Start at 6:30pm instead of 6:00pm

**More feedback?**

We really want to hear more from you: How did the session go? What did
you like? What didn't you like? What do you think we could have done
better?

Join the discussion on [discord][10], or this [Q&A board][22].

**Next session**

We're working really hard to lock down a venue for the next sessions, so
we'll keep you posted once we have that! Note that until then, the dates
on our [sessions list][23] are to be confirmed!

While you are waiting for the next session, there are a few things that
you can do!

Read select parts of the [_Mastering Ethereum_][24] book, which we'll be
discussing in the next session:

  * Chapter 1: What is Ethereum

    * Optional: _Ethereum a€™s Four Stages of Development_
    * Optional: _The Birth of Ethereum_
    * Optional: _Ethereum a€™s Development Culture_
    * Read all of the sections in this chapter, except for these ones above, as we do not plan to discuss them in the next session.
    * If you only have time to read _one_ section, read: _Ethereum and Turing Completeness_
  * Chapter 13: The Ethereum Virtual Machine

    * Optional: Compiling Solidity to EVM Bytecode
    * Optional: Contract Deployment Code
    * Optional: Disassembling the Bytecode
    * Read all of the sections in this chapter, except for these ones above, as we do not plan to discuss them in the next session.
    * If you only have time to read _one_ section, read: _Turing Completeness and Gas_

Also, please think of some ideas for a DApp that you would like to
build. Bring your ideas along to the next session. Over the course of
the sessions, we'll be helping you to refine your ideas, and build them
into DApps!

As promised, future sessions are going to be less lecture-like and more
like a technical workshop or book club!

See you all again soon!

* * *

[][25]

* * *

#### Tags

  * [irl][26]
  * [s01][27]
  * [s01e01][28]
  * [summary][29]
  * [videos][30]
  * [[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)][31]
  * [dapp][32]

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
   [13]: data:image/jpeg;base64,/9j/2wBDABALDA4MChAODQ4SERATGCgaGBYWGDEjJR0oOjM9PDkzODdASFxOQERXRTc4UG1RV19iZ2hnPk1xeXBkeFxlZ2P/2wBDARESEhgVGC8aGi9jQjhCY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2P/wgARCAAIABQDASIAAhEBAxEB/8QAFwABAAMAAAAAAAAAAAAAAAAAAAIDBP/EABQBAQAAAAAAAAAAAAAAAAAAAAL/2gAMAwEAAhADEAAAAc9AFMBf/8QAGBAAAgMAAAAAAAAAAAAAAAAAABEBAhL/2gAIAQEAAQUCdcpkH//EABYRAQEBAAAAAAAAAAAAAAAAAAABEf/aAAgBAwEBPwGNf//EABURAQEAAAAAAAAAAAAAAAAAAAEQ/9oACAECAQE/AVn/xAAaEAABBQEAAAAAAAAAAAAAAAAA[ETF](https://www.fixpro.org/post/etf-liquidity/)BUWGh/9oACAEBAAY/AkqTB+n/xAAZEAEBAQEBAQAAAAAAAAAAAAABEQAhMUH/2gAIAQEAAT8hOqL4nFGWPswJxZ//2gAMAwEAAgADAAAAEAAf/8QAFREBAQAAAAAAAAAAAAAAAAAAAQD/2gAIAQMBAT8QARP/xAAVEQEBAAAAAAAAAAAAAAAAAAABAP/aAAgBAgEBPxBEkv/EABkQAQADAQEAAAAAAAAAAAAAAAEAESExUf/aAAgBAQABPxBLCqnKtpSB7VeFMAcjvE//2Q==
   [14]: /static/3d9468cf3e8f662e5ef1c8fb13f5beaa/3df8f/dadc-s01-e01-featured-image.jpeg
   [15]: https://dappsdev.org/deck/s01e01/
   [16]: https://anders.com/[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)/
   [17]: https://twitter.com/joeytwiddle
   [18]: https://anders.com/[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)/tokens.html
   [19]: https://www.youtube.com/watch?v=-cCnIXIfULo
   [20]: https://www.youtube.com/watch?v=E-T7uLup2Js
   [21]: https://github.com/engineersftw/gitwiki
   [22]: https://app2.sli.do/event/awgvs53v/live/questions
   [23]: https://dappsdev.org/sessions/
   [24]: https://github.com/[Ethereum](https://www.playgroundfx.com/blog/the-creator-of-ethereum/)book/[Ethereum](https://www.playgroundfx.com/blog/the-creator-of-ethereum/)book
   [25]: https://dappsdev.org/blog/2019-02-25-dapps-dev-club-kickoff-session/
   [26]: /tags/irl/
   [27]: /tags/s-01/
   [28]: /tags/s-01-e-01/
   [29]: /tags/summary/
   [30]: /tags/videos/
   [31]: /tags/[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)/
   [32]: /tags/dapp/