# OmiseGO AMA 07

**[OmiseGO AMA 07 - November 23, 2018](https://www.reddit.com/r/omise_go/comments/9zuwfc/omisego_ama_7_november_23_2018/)**

***

**With the hard spoon not going forward it also casts a shadow on other claims, how can you say that something similar won't happen again?**

The main distinction here is that with the Cosmos spoon there were a lot of external dependencies, in terms of actual implementation as well what information was available to us and the way things were communicated. We made the announcement based on the information we had at the time; factors outside our jurisdiction obviously changed between then and now, but until very recently we really did believe that the spoon was going forward and were doing everything we could to facilitate that.

There would have been one possible path forward for us to keep to the storyline that started in April, which admittedly would have saved us some face: when the third party steward pulled out and Cosmos made the decision to focus solely on generalized DEX software, we could have taken on the project of building the new DEX ourselves. But that felt like an irresponsible move right now, with our own plasma DEX on Ethereum still very much under construction, and our top priority was to stay on track with our core objectives.

To address your specific items of concern, if this post isn't long enough yet, here's a recap on the state of each of those items:

DEX (Practical implementation, atomic swaps, etc.): we have a clear path forward on this, and have published details of our design, including an honest assessment of the tradeoffs we're making in the first iteration.

Network Volume as Omise is a real business: As we’ve stated before, we’ll encourage and support existing Omise customers to integrate OMG but we can’t force it upon them. It will be a gradual process - the more functionality we build into the network, the more incentive merchants will have to make the switch. That said, OMG's success is not specifically dependent on Omise's payments volume - we're also doing business development specific to OMG and OmiseGO.

PoS: this was addressed in the recent State of the Ecosystem post: "Similar to how the DEX design couldn’t really be finalized until the Plasma chain was in a pretty advanced state, it doesn’t make sense to finalize the PoS design until the DEX design has been built out to some extent. Although we have a general framework, there isn’t much to report in the meantime because that framework doesn’t really get defined in a granular way until the time comes to put it into action." The most immediate challenge with PoS is burdensome hardware and network requirements for stakers looking to run their own validator nodes on early iterations. This is something we’re looking into more deeply now so that we can put out more detailed guidance as we get closer to the PoS phase.

Very high TPS (25k, 50k, 100k and higher): this comment by Kelvin addresses tps roadblocks and is worth a full reread, with the caveat that it's from a few months back and a lot of research progress has been made since then. The gist of it is that we're focusing first on having a really solid, secure base layer capable of handling enough transactions to get the job done, and then will build in more complex functionality that will allow us to raise or eliminate the tps ceiling.

Multiple child chains: It's been a while since we talked about nested chains specifically, although it does tie in with the EVM-on-Plasma conundrum. It seemed due for a revisit so Kelvin just published a blog with a more thorough analysis. The bad news is that nested chains are more complicated than the plasma white paper implied; the good news is that it looks more and more likely that they won’t be needed. Advancements in Plasma Cash research in particular have increased the scaling potential of a single-chain construction by reducing the computational load per transaction. That research needs to be substantiated but it’s definitely a promising path right now.
As an aside: nested chains was the idea from the plasma white paper that was probably the least befuddling to the average human brain (and the one that best lent itself to visual representation), so it’s stuck in a lot of people’s minds as the defining characteristic of plasma. We’d argue the most essential feature of plasma is actually the exit game, which allows the plasma chain to maintain the security properties of Ethereum while processing transactions much more efficiently. Nested chains were just a proposal for how to cram in even more transactions, so if they go out the window in favor of a different scaling solution that is as effective or more, then it’s not much of a loss.

Cross blockchain support: on a cautious note, we’re taking this one step at a time - as specified in our post about publication of the OMG Network repo, "Tesuji Plasma is built for cheaper, faster transactions without sacrificing safety, with native support for ETH (as opposed to Wrapped Ether) and ERC20 tokens." That said cross chain support is actually pretty straightforward in the case of blockchains that can run on EVM, i.e. most chains other than Bitcoin, by using the core Ethereum chain to mint ERC20s representing tokens from other chains and depositing them into the plasma chain. As far as Bitcoin goes, the recent Wrapped BTC effort is a step in the right direction although at this point it requires federated custodianship (via a DAO, which we will participate in along with a number of other projects), which will suffice for users but is obviously a less-than-perfect solution in terms of full decentralization.

Multiple child chains (or their replacement), cross-chain support and very high tps without sacrificing security are all great examples of the kind of generalized plasma development that Kelvin in particular has been working on. Our dev team is building the infrastructure needed for our own implementation; but the ability to deploy EVM to run smart contracts on plasma, continue to increase potential tps, and support cross-chain transactions more efficiently are of pretty universal interest. At this point these are not implementation challenges specific to one project but rather research problems better solved by having as many eyes on them as possible; so our best strategy is actually to support (and contribute to) the community-wide efforts to solve these problems.

The reason that the limitations of our implementation in its current form are known is that we've been up front about what the problems we still need to solve; we share what we know about challenges. Anyone who has read posts written by Kelvin or David, or follows Kelvin on Twitter, or read the recent Coindesk article, knows that both of them have always been exceptionally candid about the state of plasma research and development.

We can't say with certainty that we'll never encounter an insurmountable obstacle. But the roadblock with the spoon wasn’t technical challenges, it was a breakdown of cooperation and communication. Unlike efforts that rely on collaboration with specific external actors, we have full visibility into our own in-house development and, for as long as OmiseGO remain its primary architects, we are the ones making decisions about its direction. To whatever extent development of OMG Network becomes a more distributed effort (something we would love to see more of), OmiseGO will always have agency to continue development regardless of anyone else’s participation.

Finally, can you expand on what you mean by difficulties with plasma research? If you're referring to the Coindesk article, we've already clarified that the statements from Kelvin and David were mischaracterized. They were referring to the need for industry-wide standards around the plasma framework (an effort we wholeheartedly support) rather than roadblocks in the specific plasma implementation being worked on by OmiseGO. If you’re talking about something else that isn’t covered above, we’ll be happy to address it.

***

**Does the OMG team have enough funding for development, even if OMG token value would drop to below $1?**

We were aware from the beginning of how volatile the crypto market can be, and have planned accordingly.

***

**OmiseGO has started a WeChat community in China. Why has OMG chosen China and what does it intend to do there?**

There is a huge and growing demand for financial services in China. Their fintech industry is massive and its blockchain scene is growing, with many experts, projects and events already established there. The interest around blockchain technology is increasing and with it, the number of blockchain tech enthusiasts and those who want to participate and contribute to the infrastructure we are building.

We view this as an opportunity to enter the Chinese market and engage with community members. Language can be a barrier which was why we started with WeChat. At this stage we are focused on building a community there, to engage and inform people about OmiseGO's activities, what the OMG Network is, its function, features and potential, and how institutions and individuals can benefit from it. We’re trying out different platforms to see what’s most conducive to building a dynamic community of developers and/or enthusiasts. We are also working to engage the developer community through activities with the Neutrino blockchain co-working space.

***

**It was discussed in Town Hall #2 that approximately the top 200 token holders would be allowed to run a full staking node. Just curious how will you enforce a fair process?**

200 validators was in reference to the staking model that was developed for the Honte milestone. Some parameters will change with proof of stake for plasma. But the core question here is, how do we keep one person, or a small number of people, from controlling the network?

We want the number of validator nodes allowed to be as large as possible without sacrificing efficiency. More validators means increased resistance to censorship or monopolistic behavior, but since the mechanism relies on a certain percentage of validators signing off on a given transaction, too many validators means unacceptable lags due to communication delays. Of course we don’t want a monopoly! But we can’t reach in and take nodes away from people that we don’t think should have them; it would be an oxymoron for a centralized party to enforce decentralization in that way. So our job is to implement a construction where there is a sufficiently distributed validator set, but the network isn’t bogged down by millions of signatures flying back and forth.

***

**With over one year of research and coding under your belts is there any reason to doubt that Plasma (OMG) will be able to reach 1,000,000 TPS?**

The plasma research community (OmiseGO and others) are still aiming for a throughput of that scale; but we’re not fixating on that specific number, which is pretty arbitrary and orders of magnitude beyond what the largest payment networks handle today. The 1 million tps figure was meant to represent that the network would be able to handle as many transactions as we could throw at it. To put it into perspective, we did some quick math: in order for 1 million tps to be necessary, every living human would have to submit roughly 11.5 transactions per day to the OMG Network.

For now we’re focusing on a solid base layer that gives us the throughput we need for real-world use without sacrificing security or decentralization. We’re entirely confident that we’ll be able to scale the network’s capacity proportional to the throughput we need.
