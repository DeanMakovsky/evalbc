# Evaluating BlockCypher's Confidence Level

Members:
*  Dean Makovsky
*  Vignesh Kuppusamy
*  Kevin Zhao
*  Joseph Tobin

We intend to test the efficacy of the confidence level provided by Blockcypher. We will test various methods of “tricking” the confidence level provided by Blockcypher in an attempt to create a fraudulent transaction that Blockcypher recognizes as having a high confidence level.  
  
# Plan

Our process for this is to first map out the entirety of the bitcoin network’s nodes and then attempt to leverage the topology in our double spending attempts. In each attempt we will monitor the confidence level and see how accurately it can predict the chance of double spends. We will attempt to then figure out what the confidence level threshold should be to accept a transaction as valid.

Our expected outcome by the end of the semester will be a report with an analysis of our attempts at tricking BlockCypher’s confidence.  The world will benefit from this by having a more accurate estimation of how much BlockCypher’s confidence level can be trusted. If we manage to find valid methods of tricking BlockCypher’s confidence level, then Blockcypher can learn from our methods and make their service more reliable as a result. We can also supply information on what the minimum threshold of confidence should be before a transaction is accepted by a merchant. If we do not manage to find any methods, then we increase, albeit marginally, the level of trust one can place in BlockCypher’s confidence level.

# Readings

Two Bitcoins at the Price of One? http://eprint.iacr.org/2012/248.pdf
An in-depth article that analyzes double spend attacks: https://medium.com/@octskyward/double-spending-in-bitcoin-be0f1d1e8008
Article on Confidence Factor: https://medium.com/blockcypher-blog/from-zero-to-hero-bitcoin-transactions-in-8-seconds-7c9edcb3b734

# Milestones
*  Send transactions to specific nodes prgramatically
*  Investigating connections between miners to create a graph of network latency between nodes.  To accomplish this, we need to understand how nodes on the Bitcoin network discover each other and how transactions propagate across the network.  To create a latency graph, we will send transactions to selected miners and wait to hear responses back from other miners.
*  Determine which nodes BlockCypher can see


#Todo
* Create node to target/bombard Blockcypher servers
* 