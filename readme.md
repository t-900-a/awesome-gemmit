# awesome-gemmit [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> aggregation and web content rating website for gemini://

![](https://siasky.net/AAB20LSkGyNNVlqu353VdREc35QDP_xmGssZlEJOFKKJeA)

[Gemmit](https://github.com/t-900-a/gemmit) relies on an ecosystem of open technologies. When using Gemmit you'll want to use tools outside of the website to upvote your favorite feeds or to read your favorite feeds.

[Project Gemini](https://gemini.circumlunar.space/)

[The Atom Syndication Format](https://tools.ietf.org/html/rfc4287)

[Monero](https://www.getmonero.org)

## Contents

- [ATOM/RSS Feeds](#atom)
  - [Generators](#generators)
  - [Readers](#readers)
    - [CLI](#cli)
    - [Mobile](#mobile) 
    - [Browser](#browser)
- [Cryptocurrencies](#cryptocurrencies)
  - [Monero](#monero)
    - [Mining](#mining)
    - [Wallets](#wallets) 
  - [Other](#other)


## ATOM/RSS Feeds

Gemmit is used to seek out great ATOM/RSS Feeds, once you find a feed you need a way to subscribe and read it.

### Generators

Note that all feeds submitted to Gemini must include a rel="payment" link.
The generators listed will need to be modified in order to include the link within the author tag. I welcome any developers to modify an existing solution or to create a new feed generator.
At this point in time it should manually be added after generation: <atom:link rel="payment" type="application/monero-paymentrequest" href="monero:donate.getmonero.org"/>

- [GMIToAtomFeed](https://github.com/LukeEmmet/GMIToAtomFeed) (Perl) - CGI script to generate an Atom feed for your Gemini log by parsing your gemlog index summary
- [Gemfeed](https://tildegit.org/solderpunk/gemfeed) (Python) -  tool for generating Atom feeds for directories of text/gemini files
- [Flounder](https://github.com/alexwennerberg/flounder) (Go) - A small site builder for the Gemini protocol, atom feeds are generated for you by the site.
### Readers
Note that no readers currently support rel="payment" links included within feeds. Until there is client support it is recommended to display the uri the feed's content
#### CLI
- [Amfora](https://github.com/makeworld-the-better-one/amfora) (Go) - gemini cli browser that includes features to subscribe to feeds
#### Mobile
- [Lagrange](https://gmi.skyjake.fi/gemlog/2021-03_testflight.gmi) - gemini mobile browser that includes features to subscribe to gemini feeds (atom/rss unsupported at this time)
#### Browser
- [Lagrange](https://github.com/skyjake/lagrange) (C) - gemini gui browser that includes features to subscribe to gemini feeds (atom/rss unsupported at this time)

Any other Feed reader would be supported, but you will have to use a Gemini to http proxy such as https://proxy.vulpes.one/ or use http feeds

## Cryptocurrencies

Readers can pay the authors/curators of feeds by paying them with cryptocurrencies.
Monero is supported at this time, any other public blockchains can easily be supported.

### Monero

Monero is private digital cash. It is a great way to tip your favorite creator. Each tip is considered a vote on Gemmit.

Gemmit requires feeds to contain a Monero address and a Monero view key.
The view key only reveals incoming transactions, outgoing transactions are kept private.
Incoming transactions need to be revealed in order to rank feeds on the site.
#### Mining
- [XMRig](https://xmrig.com/) - Monero doesn't have to be purchased, it is easy to mine with any desktop computer.
#### Wallets
- [MyMonero](https://mymonero.com/) - The MyMonero lightwallet is the quickest way to generate a wallet to start earning on Gemmit. Web, Desktop, and Mobile clients exist.
- [Official](https://getmonero.org/downloads) - The official Monero Wallet includes GUI and CLI applications

### Other
Gemmits design was sensitive to that fact that everyone has their preferred currency. Tips could be denominated in BCH or USDC, it just takes someone to build it.

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
