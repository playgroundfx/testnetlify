+++
categories = ["Cryptocurrency", "Blockchain", "SmartContract"]
date = "2019-07-14"
description = "Season 1 recap | News | undefined"
tags = ["Cryptocurrency", "Blockchain", "SmartContract"]
title = "Season 1 recap | News | undefined"
type = "post"
+++

[![DApps Dev Club][1]][2]

[Sessions][3][Partners][4][Projects][5][Certificates][6]

[![Github][7]][8][![Discord][9]][10][![RSS Feed][11]][12]

# Season 1 recap

![][13]![][14]

 __

DApps Dev Club is a technical book club, whose format is different from
most other tech meetups. Rather than have two or three speakers
delivering a short lecture about a particular topic, it is about
learning some source material (taken from _Mastering Ethereum_ , by
Gavin Wood and Andreas Antonopoulos), and then applying that in hands-on
exercises.

Also, as I'm sure to mention in every single session, these sessions
have nothing to do with investing or finance, and in fact we don't care
about the price of Ether at all (only gas price for [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)
function invocations).

We just concluded our first season, which is a series of ten sessions,
where an attendee could start off with:

  * Zero knowledge about [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)s
  * Zero knowledge about Solidity or [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s
  * Only some basic knowledge about Javascript

… and would end up with being able to build a basic DApp.

We started with our first session on the 20th of February, and just had
our final one earlier this week, on the 9th of July, running at a
**tremendous clip** of one session every two weeks.

Running all of these sessions has been quite the experience!

## Thanks

Before we get into the recap, we would like to thank everyone who made
this possible. In every session, we have been thanking the organisations
who have sponsored the events, or have helped us with community
outreach.

This time, we would like to thank the **people** who have helped out in
so many different ways.

[Dr Leong Li Ming][15] from Lifelong Learning Institute, for helping us
to navigate the world of government sponsorship. Without her savvy, we
would not have been able to get the ball rolling. DApps Dev Club is
funded by SkillsFutureSG, and is now also part of the SkillsFuture
Festival 2019 - and this would not have been possible without her advice
and constant communication.

[Ashlie Chin][16] & Dennis from Chainstack + Acronis, for being such
excellent venue hosts. Ashlie went out of her way to get the office set
up just nice for the events, and Dennis for his perfect AV set up
skills. Of course [Laurent Dedenis][17] and [Eugene Aseev][18] as well,
for providing us with their excellent office space.

[Sarah Thiam][19] & Dickson from Microsoft, for being excellent venue
hosts as well. If not for them, we would have been in quite the pickle,
and two out of the ten sessions would have had to be cancelled. Thanks
for getting us out of tricky spots in our times of need.

[Puah Hui Ying][20] & [Wong Zi Hui][21] & [Daniel Shen][22] from NBC'19,
for supporting the events in various ways. Everything from inviting
people to attend, to ad-hoc speaking, to helping out with the AV - all
these things add up. Plus, it was great organising NBC'19 with all of
you!

[Michael Cheng][23] from EngineersSG, for putting together your _git
wiki_ , and sharing all of your tech meetup recording know-how, all open
source. Starting this season involved buying about $1000 worth of AV
equipment, which is a very heavy investment, especially if you don't
know what you're doing. I certainly had no idea what I was doing, but
the EngineersSG _git wiki_ gave me the confidence that this particular
AV set up would work, and by proxy, the confidence to stump up the cash.
We have video recordings of every session, and those of you who have
**missed sessions** here and there, or heard about DApps Dev Club later
on in the season, have a way to **catch up** on them.

[Jack Ng][24], for not only **attending every session** in the whole
season, but also offering to help me out with reviewing the workshop
materials - completely voluntarily - and providing **great feedback**.
You have definitely helped improve the quality of the hands-on
exercises, and thus that of the sessions.

[Alex Towle][25], for his passion in the Ethereum education space, which
was key in the go vs no-go decision in the early stages where DApps Dev
Club was just an idea, just a concept. Subsequently too, for having
quite a few long chats with me during the planning phase, about the
sessions, helping me to formulate the entire season in advance.

[Gerald Nah][26], [Kenneth Goh][27], [Scott Koh][28], & [Solomon
Soh][29] for helping out with so many miscellaneous things, from helping
to check attendees in on the ticketing system, to helping out with
projectors, to even helping buzz people into the office space.

Not forgetting all of **you** who have attended too! Thank you for
coming to the sessions, asking great questions, eating _kueh_ together,
and even taking part in hackathons together!

You have been awesome, and it has been fun!

## Recap

We started off this season with a kickoff session where the concepts of
decentralisation, and of DApps, were introduced. Also, _minimum viable
[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)_ \- the bare minimum that you needed to know about how
[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/)s work, in order to begin developing DApps - was quite the
hit!

We then went on to introduce - conceptually - the EVM, [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s,
and web3; plus relate them to the general problems that distributed
computing tries to solve. Exploring the stack-based execution model of
the EVM appeared to generate quite a few _Aha_ s.

Subsequently we generated Ethereum keys using BIP39, and used Metamask
to send simple transactions on a test network. For many who attended
this was their **first ever interaction** with a crypto network.

At this point we had not yet even begun developing a DApp, but rather
been focused on learning about, and interacting with, some of the
building blocks of a DApp.

Next we looked at Solidity by feature, introducing the programming
language used in [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s. We also used a few new developer
tools: `solc`, Truffle, and Ganache.

Having learnt about writing [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s, we next learnt [how to](https://www.playgroundfx.com/blog/forex-trading-how-to/) test
them. This began with a crash course in Javascript testing via Mocha,
and then quickly adapting that to test various aspects of smart
contracts, using truffle's built-in test runner

A DApp is incomplete without a client, thus next we did some front end
web development, creating a bridge between in-browser Javascript and our
[smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s using `web3.js`, and used that to invoke [functions](https://www.fintechee.com/tutorial-for-forex-trading/basic-functions/) and
listen to events.

At this point we had built what we could have called our first DApp, and
it was time to switch thing up to more advanced topics.

This began by delving into the nebulous world of security. Of course, we
could not do it any justice, due to its enormous depth, and thus we
simply did an introductory level survey of various facets of security
that relate to DApps. We talked about security training games (such as
Ethernaut), modules and [Libra](https://www.playgroundfx.com/blog/libra-creator/)ries (such as OpenZeppelin), and code
analysis tools.

One of the main pain points that was highlighted very early on, in the
first few sessions, was the tremendously high cost of persistent storage
in [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)s (the `SSTORE` EVM op code). Many DApps solve this by
using IPFS, a decentralised file system, to store larger data, and files
- and so we explored this.

In our penultimate session, we tied up all the various loose ends,
things that are important to DApp development, but we had simply glossed
over in order to focus on the key parts. We talked about Infura and data
encryption. We then talked about all the various things that should be
explored if we were to go deeper, and build more complex DApps.

We concluded the season with a bang - after nine sessions in a row with
just me talking, we had our final one with a much more exciting line up,
featuring three guest speakers. All of them talked about different
aspects of DApps and decentralisation in general, that was _beyond_
Ethereum.

## Next season

DApps Dev Club is _planning_ to hold its next ~~session~~ season soon!

… but we would like to hear from you first!

  * What are the other networks that you would like to build DApps on?
  * Are there any upcoming hackathons that you would like to build a DApp at?
  * What would you like to learn about in DApps Dev Club season #2?
  * Do you have a venue that we can use for session in season #2?
  * Do you have cash to splash to sponsor sessions in season #2?

Please join the [DApps Dev Club chat group][30] and let me know your
answers to the above.

* * *

[][31]

* * *

#### Tags

  * [irl][32]
  * [s01][33]
  * [recap][34]
  * [thanks][35]

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
   [13]: data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAFCAYAAABFA8wzAAAACXBIWXMAAC4jAAAuIwF4pT92AAABGUlEQVQY02NIjpyd7G3f99/HoXt1YtjME35OvVdCvSZp56ctavZz7t3rZdf1OT5kxsoQzwnvshOWhDMwMAgxM7NGAOkoIHYF4kggtgZibSDmZkiNnhPg69izAYg3+jv3PgYaeMrBpGUmkP8w0LW/O8x70iqgBa+j/KdkATUw8HDK8wMpLSBWBWIpIJYHYi4oZgYZGO9q2f4e6MLjoZ4TvwHpZ9lJC+bmpS4qdDZvm+9t3/0i0m8KyOV30uNme4MMZWPl1AFSIFcaAbEpEFsxwEBK1Gw7D5vOvbFB06JTomcXJITNrGxv2BQLkgO6sh7o5aUNFWvlQr0mtiaETVMBibOwsEsDKRsgNgNiTyD2AmJGBnKAvkYIXo0Ap79aRtHLd6wAAAAASUVORK5CYII=
   [14]: /static/2bc977b3e5ba2cb5948bf2f9e478586f/d0869/dadc-s01-recap.png
   [15]: https://www.linkedin.com/in/limingleong/
   [16]: https://www.linkedin.com/in/ashlie-chin-b74b8491/
   [17]: https://www.linkedin.com/in/laurent-dedenis/
   [18]: https://www.linkedin.com/in/easeev/
   [19]: https://www.linkedin.com/in/sarahthiam/
   [20]: https://www.linkedin.com/in/puahhuiying/
   [21]: https://www.linkedin.com/in/zihui-wong-4bab10a5/
   [22]: https://www.linkedin.com/in/dansjd/
   [23]: https://www.linkedin.com/in/miccheng/
   [24]: https://www.linkedin.com/in/jack-ng-b2593b151/
   [25]: https://www.linkedin.com/in/alex-towle-937647144/
   [26]: https://www.linkedin.com/in/geraldnahhawyuan/
   [27]: https://www.linkedin.com/in/kenneth-goh-65ba9525/
   [28]: https://www.linkedin.com/in/scottkohzhiwei/
   [29]: https://www.linkedin.com/in/solomon-soh-zhe-hong/
   [30]: https://bit.ly/dadc-chat
   [31]: https://dappsdev.org/blog/2019-07-14-dapps-dev-club-season-1-recap/
   [32]: /tags/irl/
   [33]: /tags/s-01/
   [34]: /tags/recap/
   [35]: /tags/thanks/