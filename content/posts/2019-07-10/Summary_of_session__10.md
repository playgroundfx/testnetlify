+++
categories = ["Cryptocurrency", "Blockchain", "SmartContract"]
date = "2019-07-10"
description = "Summary of session #10"
tags = ["Cryptocurrency", "Blockchain", "SmartContract"]
title = "Summary of session #10"
type = "post"
+++

[![DApps Dev Club][1]][2]

[Sessions][3][Partners][4][Projects][5][Certificates][6]

[![Github][7]][8][![Discord][9]][10][![RSS Feed][11]][12]

# Summary of session #10

![][13]![][14]

 _Finale session, featuring guest speakers on permissioned networks,
verifiable credentials, and non-[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/) DLTs_

The DApps Dev Club held its tenth session - the **final one** for the
first season - featuring three **guest speakers** :

  * Thomas Lee from Chainstack
  * Wong Wai Chung from NextID
  * Calvin Cheng from Hedera Hashgraph

We spent sessions one through nine covering topics that were focused
very much on Ethereum, and developing decentralised applications using
Ethereum. In this finale session though, we took a different track - and
our topics were all themed around _Beyond Ethereum_. The common thread
between all of the different topics was how technology and concepts
employed by Ethereum, or other crypto networks, have been used in
different ways.

We also had a **record high turnout** for the session: 44!

~~Videos will be posted soon!~~ All [videos from this session][15] have
now been posted!

## Format

The usual format for our sessions thus far has been:

  * Cover material selected from _Mastering Ethereum_
  * Try out a demo, or do a hands-on exercise
  * Repeat the above a two or three times

This time however, we had no hands-on exercises, and we had guest
speakers talk about their experiences. The format was more similar to
the usual tech meetup format. It was nice to change things up a little!

## Above and beyond

During the sessions, we thanked not only the organisations that have
made the sessions possible, but also the individual people who have gone
out of their way to help out with running them.

A quick shout out to: Dr Leong Li Ming from Lifelong Learning Institute,
Ashlie & Dennis from Chainstack & Acronis, Sarah Thiam & Dickson from
Microsoft, Wing & Daniel & Lewis from NBC'19, Michael Cheng from
EngineersSG, Gerald Nah, Kenneth Goh, Jack Ng, Scott Koh, Solomon Soh -
all of you have helped out in many ways that are mostly behind-the-
scenes, and thus often unnoticed. You have been great, and helped make
these sessions happen!

## Topics

### Permissioned networks and Quorum

[Thomas Lee][16] from Chainstack kicked off the session with a talk
about permissioned networks, with a focus on Quorum.

Quorum is a fork of Ethereum, with modifications made that make it
suitable for deployments in permissioned networks - which are also known
as private chains. The key changes that Quorum has made to Ethereum are
that:

  * It uses a different consensus algorithm (RAFT or IBFT) instead of Proof-of-Work (Satoshi consensus)
  * It has the concept of a private transaction - referred to as `privateFor` in Quorum lingo - where data is encrypted at rest, and public key cryptography is used to gate read and write access to [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/) data

Thomas explored the implications of each of these differences in depth.

My personal reflection here is that while permissioned networks are _not
truly decentralised_ , they still have some of the benefits of using the
technologies that underpin crypto networks, in order to build general
purpose _distributed computation networks_.

### Structured documents, verifiable credentials, and self-sovereign
identity

[Wong Wai Chung][17] from NextID talked about structured documents,
verifiable credentials, and self-sovereign identity.

So we started off with structured documents, which are essentially
representing something in a manner that is machine parseable, because it
has a schema, and the schema itself is defined using a standard - in
this case that standard was JSON-LD.

However, the problem with structured documents is that they only solve
parseability - anyone can make up fake data that passes schema
validation. For this, we need verifiable credentials. Think checksums,
except instead of CRCs, weighted-modulos, et cetera, you use hash
[functions](https://www.fintechee.com/tutorial-for-forex-trading/basic-functions/), Merkle trees, and write the Merkle tree's root onto an
immutable distributed ledger (Blockchain, for example).

This certainly guarantees you a lot more than just having structured
documents, but you could still make up _fake credentials_ , you would
just need to do a bunch of extra steps in order to have it validate.
This is where we need to use digital signature [algorithms](https://www.fintechee.com/algorithms-for-trading/) in order to
ensure that a document is indeed not made up, as we know that only the
possessor of a particular private key can sign data.

And yet again, we find a hole in the solution, because anyone can
_generate their own set of keys_ and claim themselves to be the signing
authority, and sign their own documents, thereby passing all of the
validations necessary. At this point it becomes apparent that the core
issue that needs to be solved really is **identity**. When a claim of an
identity is correctly independently verifiable, then we can plug the
final whole in the sequence of solutions that we have gotten up to with
at this point.

This was certainly a meaty talk, with lots of completely new concepts
introduced.

My personal takeaway from this was that identity is a problem that is
hard to solve, and that we have yet to find a solution that is self-
sovereign, that is, not based around blind trust in a central authority.
The path taken to solving this problem, however, already has lots of
interesting solutions.

### Non-[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/) distributed ledger technologies

[Calvin Cheng][18] from Hedera Hashgraph talked about non-[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)
distributed ledger technologies.

Hashgraph is both a consensus algorithm and data structure. It has been
used to build Hedera, which is a crypto currency, that does _not_ use
[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/) at all:

  * For **consensus** : Instead of using Proof of Work, an alternate "gossip about gossip" voting based consensus algorithm is used instead.
  * For **data structures** : Instead of having a singly linked list where each node is a binary tree of transactions, a directed acyclic graph where each edge is a transaction is used instead.

This in itself turns everything we know about crypto currency
implementation on its head, as two core parts of their implementation
have been completely replaced by something radically different. It is a
distributed ledger technology that is _not_ a Blockchain.

What's interesting is that despite these differences, development of
DApps is not going to be that much different, because their smart
contracts are based on the EVM, and plan to be compatible with Ethereum
dev tools and [Libra](https://www.playgroundfx.com/blog/libra-creator/)ries, such as Truffle and `web3.js`.

My personal takeaway here was that DApp development skills are
transferrable from one crypto network to the next - at least some of the
time. Furthermore, that the existence of such a radically different
network implementation is evidence that there is a huge amount of
innovation in technologies used in decentralisation, and we are likely
only just beginning to see this space mature.

## Next season

DApps Dev Club is _planning_ to hold its next ~~session~~ season soon!

a€¦ but we would like to hear from you first!

  * What are the other networks that you would like to build DApps on?
  * Are there any upcoming hackathons that you would like to build a DApp at?
  * What would you like to learn about in DApps Dev Club season #2?
  * Do you have a venue that we can use for session in season #2?
  * Do you have cash to splash to sponsor sessions in season #2?

Please join the [DApps Dev Club chat group][19] and let me know your
answers to the above.

* * *

[][20]

* * *

#### Tags

  * [irl][21]
  * [s01][22]
  * [s01e10][23]
  * [summary][24]
  * [permissioned-networks][25]
  * [quorum][26]
  * [json-ld][27]
  * [structured-documents][28]
  * [verifiable-credentials][29]
  * [identity][30]
  * [[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)][31]
  * [consensus][32]
  * [byzantine-fault-tolerance][33]
  * [gossip][34]

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
   [13]: data:image/jpeg;base64,/9j/2wBDABALDA4MChAODQ4SERATGCgaGBYWGDEjJR0oOjM9PDkzODdASFxOQERXRTc4UG1RV19iZ2hnPk1xeXBkeFxlZ2P/2wBDARESEhgVGC8aGi9jQjhCY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2P/wgARCAAEABQDASIAAhEBAxEB/8QAFgABAQEAAAAAAAAAAAAAAAAAAAUE/8QAFAEBAAAAAAAAAAAAAAAAAAAAAP/aAAwDAQACEAMQAAABpYwpg//EABgQAQEAAwAAAAAAAAAAAAAAAAECAAMR/9oACAEBAAEFAqhyhN0xw//EABQRAQAAAAAAAAAAAAAAAAAAABD/2gAIAQMBAT8BP//EABQRAQAAAAAAAAAAAAAAAAAAABD/2gAIAQIBAT8BP//EABsQAAEEAwAAAAAAAAAAAAAAAAABAhJxMjOR/9oACAEBAAY/Atj+kZusyctn/8QAGRAAAgMBAAAAAAAAAAAAAAAAAAERIVEx/9oACAEBAAE/IZzaTLCD2RZ2bE0f/9oADAMBAAIAAwAAABCID//EABQRAQAAAAAAAAAAAAAAAAAAABD/2gAIAQMBAT8QP//EABQRAQAAAAAAAAAAAAAAAAAAABD/2gAIAQIBAT8QP//EABkQAQADAQEAAAAAAAAAAAAAAAEAESExQf/aAAgBAQABPxA27Wg0W8Mg7US0nPGozitXdryf/9k=
   [14]: /static/eb75897951b55813f7b778844811c53d/0fa5c/dadc-s01e10-roundup.jpeg
   [15]: /blog/2019-07-12-dapps-dev-club-10th-session-videos/ (Videos from DApps Dev Club session #10)
   [16]: https://www.linkedin.com/in/thomas-lee-95b024b1/
   [17]: https://www.linkedin.com/in/wai1chung/
   [18]: https://www.linkedin.com/in/calvinchengx/
   [19]: https://bit.ly/dadc-chat
   [20]: https://dappsdev.org/blog/2019-07-10-dapps-dev-club-10th-session-roundup/
   [21]: /tags/irl/
   [22]: /tags/s-01/
   [23]: /tags/s-01-e-10/
   [24]: /tags/summary/
   [25]: /tags/permissioned-networks/
   [26]: /tags/quorum/
   [27]: /tags/json-ld/
   [28]: /tags/structured-documents/
   [29]: /tags/verifiable-credentials/
   [30]: /tags/identity/
   [31]: /tags/[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)/
   [32]: /tags/consensus/
   [33]: /tags/byzantine-fault-tolerance/
   [34]: /tags/gossip/