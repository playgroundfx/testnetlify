+++
categories = ["Cryptocurrency", "Blockchain", "SmartContract"]
date = "2019-04-12"
description = "Summary of session #04"
tags = ["Cryptocurrency", "Blockchain", "SmartContract"]
title = "Summary of session #04"
type = "post"
+++

[![DApps Dev Club][1]][2]

[Sessions][3][Partners][4][Projects][5][Certificates][6]

[![Github][7]][8][![Discord][9]][10][![RSS Feed][11]][12]

# Summary of session #04

![][13]![][14]

 _Solidity: Solidity-by-feature + solc + ganache + truffle_

We held our 4th session - on Solidity - a few days ago, on Tuesday
evening at Chainstack. We covered features of Solidity as a programming
language, as well as a few development tools used to work with Solidity
- solc, truffle, and ganache.

~~We will be posting about our videos soon!~~ We have posted [our videos
from this session][15] now.

As mentioned in the [session info][16] prior to the session, we did not
manage to cover Solidity as planned in the previous session, so in this
session we covered both Solidity, and the development tools used to work
with it. So there was a lot to cover - but we got there!

## Format

As promised in the [kickoff session][17], and the sessions since, we
have transitioned from a lecture-style session, to a participatory
hands-on workshop type of session. This time apart from the
_introduction_ and _recap_ parts at the beginning, and the _next
session_ part at the end, _all_ the other parts had a hands-on component
to it.

## Difficulty and pace

During the break in the middle of the session, some of you said that the
hands-on part that we did was too easy - it was literally copy-and-paste
- and I told you to hang on till the end of the session.

In the second half of the session, we had two more hands-on parts. The
final one, the one where we used truffle, was clearly challenging, as
many of you got stuck, and needed help/ troubleshooting.

This was as intended - we want everybody to come away feeling like they
have learnt something, and accomplished something. That means making
parts of the session easy, and parts of it hard.

It was great to see that a few of you who had "figured it out" went on
to help others around you that happened to be stuck, to also "figure it
out". We really would love to see this trend continue, with you all
reinforcing each others' learning.

In this session, due to the sheer amount of content that we had to
cover, we had to pick up the pace significantly compared to the previous
sessions. Even then, we managed to run over time. Thank you everyone for
sticking around till late that that - and on a lighter note, we're glad
that we managed keep your collective attention for so long!

In fact some of you were so engaged that you were still [chatting][18]
about the topics for the night till after midnight!

## Topics

### Solidity-by-feature

  * [Deck][19]
  * [Hands-on][20]

Here we built up a very basic [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/) from scratch, feature by
feature. But not by feature of the contract, but rather by feature of
the programming language.

We started off with a basic structure of a contract that did nothing.
Then added some state variables directly to the contract using primitive
types. Next we introduced dynamic types, using a `struct` to group
several primitive type variables together, and a `mapping` to store them
as a state variable on the contract. After this, we added [functions](https://www.fintechee.com/tutorial-for-forex-trading/basic-functions/) to
add and modify those `struct`s. Then refactored the [functions](https://www.fintechee.com/tutorial-for-forex-trading/basic-functions/) to make
use of function modifiers to reduce the repetition when defining pre-
conditions that were common or similar between the [functions](https://www.fintechee.com/tutorial-for-forex-trading/basic-functions/). Finally,
we defined an `event` and wrote a new function that emitted it.

We also had a little aside, where we discussed what the term _contract_
within _[smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/)_ meant, in the context of _design by contract_ ,
as defined by Eiffel (another programming language).

### solc

  * [Deck][21]
  * [Hands-on][22]

Here we installed _solc_ , the solidity compiler, and ran it on the
command line (within a shell or terminal), with various [options](https://www.fixpro.org/post/options-liquidity/) to see
the different stages and outputs of the compiler, briefly exploring what
each was.

Here some of us ran into issues with installing _solcjs_ , and those
same issues cropped up again later on when installing _truffle_. Thanks
to Jeremy for identifying the root cause of this - turns out it had
nothing to do with either _solcjs_ or _truffle_ , but rather to do with
python 2 vs python 3. When installing them, these rely on _node-gyp_ ,
which expects python 2, but crashes when python 3 is used.The solution
was to ensure that python 2 was first on your `PATH` environment
variable. This is something to keep in mind for future sessions.

### ganache

  * [Deck][23]

This was a really short section, and it was mostly about installing the
tool and running it. Apart from that though, the larger discussion was
about how the various tools fit together in the development, deployment,
and running of decentralised applications.

### truffle

  * [Deck][24]
  * [Hands-on][25]

Here we used the [smart contract](https://www.letsplayfx.com/blog/smart-contract-on-blockchain/) that we had built earlier, and took them
for a spin. We initialised a blank truffle project, put the contract
into it. Used truffle to compile, deploy, and interact with the smart
contract, through its REPL (read-eval-print-loop).

This was the most challenging part of the session, and also where the
most problems encountered, and questions were. Also simultaneously
seemed to be the favourite part for everyone.

For those using Windows, Jack has a tip: Use `truffle.cmd` instead of
`truffle` in order to avoid certain errors.

An astute observation, from Joey, was:

> I saw there were three levels of payment:

>

>   * contract.numCars.call() is free (just querying the node's chain I
guess)

>   * contract.honkCar() costs some gas

>   * contract.addCar() costs some gas, and the contract also demands
that you send it some Eth!

>

That is spot on - when calling a function that does not change the state
of the contract in any way, query the local copy of the contract, rather
than query the copy of the contract that is on the [blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/).

When you do execute a function on a copy of the contract that is on the
[blockchain](https://www.letsplayfx.com/blog/trade-forex-with-bitcoin/), that must be done through a transaction. Any transaction
that gets executed requires a certain amount of gas to run (depending on
its computational complexity), and that gas must be paid for in Ether,
otherwise, none of the Ethereum nodes in the network will execute the
transaction, as the incentive to execute the other transactions will
mean that they will be prioritised. So the nodes performing the
transactions must always get their fee.

Over and above this, optionally, the transaction may also send ether to
the contract itself. In Solidity, this means that the function must be
marked with the `payable` keyword. When this is present `msg.value`
amount of Ether is added to the contract.

Another observation, also from Joey, was an error on my part.

    
    
    contract.numCars() // should cost ETH
    contract.numCars.call() // should be free

However, it turns out that `truffle-contract`, which is truffle's own
wrapper around a deployed instance of a contract, does some _framework
magic_ here, and when the function is _view_ or _pure_ , it
automatically switches to the `.call()` variant instead of the one that
you called.

Thanks for the attention to detail and catching that one!

## Javascript??

[ ![I can haz Javascript?][26] ][27]

In the next session, we will need to come into it knowing some basic
Javascript, as we will be writing tests using mocha, to test our smart
contracts. We've posted a list of resources of where you can learn
Javascript from.

But let's face it - nothing beats some hands-on help when you're stuck
on something. So we have enlisted the _help of some volunteers_ from the
SingaporeJS community, as well as the broader developer community here.
That will certainly help for those of you attending. Hopefully it will
also make it _less_ daunting for those of you who will be doing
Javascript for the first time.

## Thanks

Thanks to [Lifelong Learning Institute (SkillsFutureSG)][28] for
sponsoring us via their learning circles program - you have them to
thank for the F&B. Thanks [Dr Leong Li-Ming][29], their principal
manager, for attending too.

Thanks to [Chainstack][30] and [Acronis][31] for hosting us at their
excellent office. Thanks [Ashlie][32] for helping us run the event, and
Dennis for putting together the excellent AV set up.

Thanks to Zi Hui and Wing as well, for their on-site assistance running
the event.

## Next session

RSVPs are now open - please let us know if you're attending, as it helps
us plan for seating, ordering F&B, etc:

[**RSVP** on eventbrite][33]

See you all again soon!

* * *

[][34]

* * *

#### Tags

  * [irl][35]
  * [s01][36]
  * [s01e04][37]
  * [summary][38]
  * [solidity][39]
  * [solc][40]
  * [truffle][41]
  * [ganache][42]

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
   [13]: data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAFCAYAAABFA8wzAAAACXBIWXMAAAsSAAALEgHS3X78AAABdElEQVQY02NgIAC+vbspeOTwfqXtWzcanjx2Qm7r9r0eFy5cNbl595H0799fhE6cOed8/vIts5evXiu8fvmUn6G6tX7Btu2r5rZPmD5z5Zr1bcnJya09Pb39a9aun3rswKbKh5c2f+zp7v5laun6ZfLkqSWVtY3/cyo7/3VOWfKta+LiN82TlvzPrWr/l5pZ8SMpteA9g4uD3f/M3ML/cVk1/0uqe/87uXj+P3Xq+H8QuHDh/JZVs8q/5KXH/pdXNvpXU1s7Pzo6/n9gaPJ//5DU/znlk//Hplb+D4pO/x8RlvrfwNDuP0NnTt4MZ5/oOREJ+XOLy1umFBbmT9i6bVP7jZtXazdt3hYTEx372t8v8E94aOTLmTOmbo2Mjv6Qmpj4LSY2739Jy6J/KZl5rxLiUr+k+cT8dfOL/08oCBlmzZxtsW7tGp2TJ09ITJvSz/Xm+V3xY0cOand097nMnLfC+unrN0IHd21UmzJjofmU+es9ASTsw9SbyDoAAAAAAElFTkSuQmCC
   [14]: /static/a9e2610edd858deb7f4e95981c183b99/4ac1b/dadc-s01e04-roundup.png
   [15]: /blog/2019-04-13-dapps-dev-club-4th-session-videos/
   [16]: /blog/2019-04-06-dapps-dev-club-4th-session-info/
   [17]: https://dappsdev.org/blog/2018-02-25-dapps-dev-club-kickoff-session/
   [18]: https://bit.do/dadc-chat
   [19]: /deck/s01e04/#solidity
   [20]: /hands-on/solidity-intro/
   [21]: /deck/s01e04/#solc
   [22]: /hands-on/solc-intro
   [23]: /deck/s01e04/#ganache
   [24]: /deck/s01e04/#truffle
   [25]: /hands-on/truffle-intro/
   [26]: /static/5ea4f60ebe46c88b4f8802224382d6e6/2fc74/i-can-haz-javascript.jpeg ()
   [27]: /static/5ea4f60ebe46c88b4f8802224382d6e6/2fc74/i-can-haz-javascript.jpeg
   [28]: https://www.lli.sg/
   [29]: https://www.linkedin.com/in/limingleong/
   [30]: https://chainstack.com/
   [31]: https://www.acronis.com/
   [32]: https://www.ashliechin.com/
   [33]: https://www.eventbrite.com/e/dapps-dev-club-session-05-testing-smart-contracts-tickets-60041615087
   [34]: https://dappsdev.org/blog/2019-04-12-dapps-dev-club-4th-session-roundup/
   [35]: /tags/irl/
   [36]: /tags/s-01/
   [37]: /tags/s-01-e-04/
   [38]: /tags/summary/
   [39]: /tags/solidity/
   [40]: /tags/solc/
   [41]: /tags/truffle/
   [42]: /tags/ganache/