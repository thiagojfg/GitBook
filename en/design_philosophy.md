# Design philosophy

These are the core tenets that sparked the work on Ethereum's architeture and implementation.

## Simplicity
The Ethereum protocol should be as simple as possible, even at the cost of some data storage inefficiency or time inefficiency. An average programmer should ideally be able to follow and implement the entire specification, so as to eventually help minimize the influence that any specific individual or elite group can have on the protocol and furthering the vision of Ethereum as a protocol that is open to all. Optimizations which add complexity should not be included unless they provide very substantial benefit.

## Universality 
It is a fundamental part of Ethereum’s design philosophy that Ethereum does not have “features”. Instead, Ethereum provides an internal Turing-complete scripting language which you can use to construct any smart contract or transaction type that can be mathematically defined. Want to invent your own financial derivative? With Ethereum, you can. Want to make your own currency? Set it up as an Ethereum contract. Want to set up a full-scale Daemon or Skynet? You may need to have a few thousand interlocking contracts, and be sure to feed them generously, to do that, but nothing is stopping you.

## Modularity 
Different parts of the Ethereum protocol should be designed to be as modular and separable as possible. Over the course of development, it should be easy to make a small protocol modification in one place and have the application stack continue to function without any further modification. Innovations such as Dagger, Patricia trees and RLP should be implemented as separate libraries and made to be feature-complete even if Ethereum does not require certain features so as to make them usable in other protocols as well. Ethereum development should be maximally done so as to benefit the entire cryptocurrency ecosystem, not just itself.

## Non-Discrimination 
The protocol should not attempt to actively restrict or prevent specific categories of usage, and all regulatory mechanisms in the protocol should be designed to directly regulate the harm, not attempt to oppose specific undesirable applications. You can even run an infinite loop script on top of Ethereum for as long as you are willing to keep paying the per-computational-step transaction fee for it.

## Agility 
Details of the Ethereum protocol are not set in stone. Although we will be extremely judicious about making modifications to high-level constructs such as the C-like language and the address system, computational tests later on in the development process may lead us to discover that certain modifications to the algorithm or scripting language will substantially improve scalability or security. If any such opportunities are found, we will make use of them.
