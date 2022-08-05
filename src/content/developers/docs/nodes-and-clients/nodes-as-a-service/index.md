---
title: Nodes as a service
description: An entry-level overview of node services, the pros and cons, and popular providers.
lang: en
sidebar: true
sidebarDepth: 2
preMergeBanner: true
---

## Introduction {#Introduction}

Running your own [Ethereum node](/developers/docs/nodes-and-clients/#what-are-nodes-and-clients) can be challenging, especially when getting started or while scaling fast. There are a [number of services](#popular-node-services) that run optimized node infrastructures for you, so you can focus on developing your application or product instead. We'll explain how node services work, the pros and cons for using them and list providers if you are interested in getting started.

**Note: it has been common for users to run consensus clients locally and use a node-as-a-service provider in place of a local execution client. This will not be possible at The Merge - users will be required to run BOTH clients locally. Users relying on node-as-a-service providers for their consensus clients will not merge correctly and will not be able to follow the Ethereum chain. Now is the time to install a local execution client!**

## Prerequisites {#prerequisites}

If you don't already have an understanding of what nodes and clients are, check out [Nodes and clients](/developers/docs/nodes-and-clients/).

## How do node services work? {#how-do-node-services-work}

Node service providers run distributed node clients behind the scenes for you, so you don't have to.

These services typically provide an API key that you can use to write to and read from the blockchain. They often include access to [Ethereum testnets](/developers/docs/networks/#ethereum-testnets) in addition to Mainnet.

Some services offer you your own dedicated node that they manage for you, while others use load balancers to distribute activity across nodes.

Almost all node services are extremely easy to integrate with, involving one line changes in your code to swap out your self hosted node, or even switch between the services themselves.

Often times node services will run a variety of [node clients](/developers/docs/nodes-and-clients/#execution-clients) and [types](/developers/docs/nodes-and-clients/#node-types), allowing you to access full and archive nodes in addition to client specific methods in one API.

It's important to note that node services do not and should not store your private keys or information.

## What are the benefits of using a node service? {#benefits-of-using-a-node-service}

The main benefit for using a node service is not having to spend engineering time maintaining and managing nodes yourself. This allows you to focus on building your product rather than having to worry about infrastructure maintenance.

Running your own nodes can be very expensive from storage to bandwidth to valuable engineering time. Things like spinning up more nodes when scaling, upgrading nodes to the latest versions, and ensuring state consistency, can distract from building and spending resources on your desired web3 product.

## What are the cons of using a Node Service? {#cons-of-using-a-node-service}

By using a node service you are centralizing the infrastructure aspect of your product. For this reason, projects that hold decentralization to the upmost importance might prefer self-hosting nodes rather than outsourcing to a 3rd party.

Read more about the [benefits of running your own node](/developers/docs/nodes-and-clients/#benefits-to-you).

## Popular node services {#popular-node-services}

Here is a list of some of the most popular Ethereum node providers, feel free to add any that are missing! Each node service offers different benefits and features in addition to free or paid tiers, you should investigate which ones best suit your needs prior to making a decision.

- [**Alchemy**](https://alchemy.com/)
  - [Docs](https://docs.alchemyapi.io/)
  - Features
    - Largest free tier with 300M compute units per month (~30M getLatestBlock requests)
    - Multichain support for Polygon, Starknet, Optimism, Arbitrum
    - Powering ~70% of the largest Ethereum dapps and DeFi transaction volume
    - Real-time webhook alerts via Alchemy Notify
    - Best-in-class support and reliability / stability
    - Alchemy's NFT API
    - Dashboard with Request Explorer, Mempool Watcher, and Composer
    - Integrated testnet faucet access
    - Active Discord builder community with 18k users
- [**Ankr**](https://www.ankr.com/)
  - [Docs](https://docs.ankr.com/)
  - Features
    - Ankr Protocol - open access to Public RPC API endpoints for 8+ chains
    - Load balancing and node health monitoring for a fast and reliable gateway to the nearest available node
    - Premium tier enabling WSS endpoint and uncapped rate limit
    - One-click full node and validator node deployment for 40+ chains
    - Scale as you go
    - Analytics tools
    - Dashboard
    - RPC, HTTPS and WSS endpoints
    - Direct support
- [**BlockDaemon**](https://blockdaemon.com/)
  - [Docs](https://ubiquity.docs.blockdaemon.com/)
  - Benefits
    - Dashboard
    - Per node basis
    - Analytics
- [**Chainstack**](https://chainstack.com/)
  - [Docs](https://docs.chainstack.com/)
  - Features
    - Free shared nodes
    - Shared archive nodes
    - GraphQL support
    - RPC and WSS endpoints
    - Dedicated full and archive nodes
    - Fast sync time for dedicated deployments
    - Bring your cloud
    - Pay-per-hour pricing
    - Direct 24/7 support
- [**DataHub**](https://datahub.figment.io)
  - [Docs](https://docs.figment.io/)
  - Features
    - Free tier option with 3,000,000 reqs/month
    - RPC and WSS endpoints
    - Dedicated full and archive nodes
    - Auto-Scaling (Volume Discounts)
    - Free archival data
    - Service Analytics
    - Dashboard
    - Direct 24/7 Support
    - Pay in Crypto (Enterprise)
- [**GetBlock**](https://getblock.io/)
  - [Docs](https://getblock.io/docs/get-started/authentication-with-api-key/)
  - Features
    - Access to 40+ blockchain nodes
    - 40K free daily requests
    - Unlimited number of API keys
    - High connection speed at 1GB/sec
    - Trace+Archive
    - Advanced analytics
    - Automated updates
    - Technical support
- [**InfStones**](https://infstones.com/)
  - Features
    - Free tier option
    - Scale as you go
    - Analytics
    - Dashboard
    - Unique API endpoints
    - Dedicated full nodes
    - Fast sync time for dedicated deployments
    - Direct 24/7 support
    - Access to 50+ blockchain nodes
- [**Infura**](https://infura.io/)
  - [Docs](https://infura.io/docs)
  - Features
    - Free tier option
    - Scale as you go
    - Paid archival data
    - Direct Support
    - Dashboard
- [**Kaleido**](https://kaleido.io/)
  - [Docs](https://docs.kaleido.io/)
  - Features
    - Free startier tier
    - One-click Ethereum node deployment
    - Customizable clients and algorithms (Geth, Quorum & Besu || PoA, IBFT & Raft)
    - 500+ administrative and service APIs
    - RESTful interface for Ethereum transaction submission (Apache Kafka backed)
    - Outbound streams for event delivery (Apache Kafka backed)
    - Deep collection of "off-chain" and ancillary services (e.g. bilateral encrypted messaging transport)
    - Straightforward network onboarding with governance and role-based access control
    - Sophisticated user management for both administrators and end users
    - Highly scalable, resilient, enterprise-grade infrastructure
    - Cloud HSM private key management
    - Ethereum Mainnet Tethering
    - ISO 27k and SOC 2, Type 2 certifications
    - Dynamic runtime configuration (e.g. adding cloud integrations, altering node ingresses, etc.)
    - Support for multi-cloud, multi-region and hybrid deployment orchestrations
    - Simple hourly SaaS-based pricing
    - SLAs and 24x7 support
- [**Moralis**](https://moralis.io/)
  - [Docs](https://docs.moralis.io/)
  - Features
    - Free shared nodes
    - Free shared archive nodes
    - Privacy focused (no logs policy)
    - Cross chain support
    - Scale as you go
    - Dashboard
    - Unique Ethereum SDK
    - Unique API endpoints
    - Direct, technical support
- [**Pocket Network**](https://www.pokt.network/)
  - [Docs](https://docs.pokt.network/home/)
  - Features
    - Decentralized RPC Protocol and Marketplace
    - 1M Requests Per Day Free Tier (per endpoint, max 2)
    - [Public Endpoints](https://docs.pokt.network/home/resources/public-rpc-endpoints)
    - Pre-Stake+ Program (if you need more than 1M requests per day)
    - 15+ Blockchains Supported
    - 6400+ Nodes earning POKT for serving applications
    - Archival Node, Archival Node w/ Tracing, & Testnet Node Support
    - Ethereum Mainnet Node Client Diversity
    - No Single Point of Failure
    - Zero Downtime
    - Cost-Effective Near-Zero Tokenomics (stake POKT once for network bandwidth)
    - No monthly sunk costs, turn your infrastructure into an asset
    - Load-Balancing built into the Protocol
    - Infinitely scale the number of requests per day and nodes per hour as you go
    - The most private, censorship-resistant option
    - Hands-on developer support
    - [Pocket Portal](https://bit.ly/ETHorg_POKTportal) dashboard and analytics
- [**QuickNode**](https://www.quicknode.com)
  - [Docs](https://www.quicknode.com/docs/)
  - Features
    - Industry-leading performance and reliability
    - 24/7 technical support & dev Discord community
    - Geo-balanced, multi cloud/metal, low-latency network
    - Multichain support (Optimism, Arbitrum, Polygon + 11 others)
    - Middle-layers for speed & stability (call routing, cache, indexing)
    - Smart-Contract monitoring via Webhooks
    - Intuitive dashboard, analytics suite, RPC composer
    - Advanced security features (JWT, masking, whitelisting)
    - NFT data and analytics API
    - [SOC2 Certified](https://www.quicknode.com/security)
    - Suitable for Developers to Enterprises
- [**Rivet**](https://rivet.cloud/)
  - [Docs](https://rivet.readthedocs.io/en/latest/)
  - Features - Free tier option - Scale as you go -[**SenseiNode**](https://senseinode.com)
  - [Docs](https://docs.senseinode.com/)
  - Features
  - Dedicated and Share nodes
  - Dashboard
  - Hosting off AWS on multiple hosting providers accross different locations in Latin America
  - Prysm and Lighthouse clients
- [**SettleMint**](https://console.settlemint.com/)
  - [Docs](https://docs.settlemint.com/)
  - Features
    - Free trial
    - Scale as you go
    - GraphQL support
    - RPC and WSS endpoints
    - Dedicated full nodes
    - Bring your cloud
    - Analytics tools
    - Dashboard
    - Pay-per-hour pricing
    - Direct support

- [**Zeeve**](https://www.zeeve.io/)
 - [Docs](https://zeeve.readthedocs.io/en/latest/)
    - Benefits
    - Dashboard
    - Per node basis
    - Analytics


- [**Watchdata**](https://watchdata.io/)
  - [Docs](https://docs.watchdata.io/)
  - Features
    - Data reliability
    - Uninterrupted connection with no downtime
    - Process automation
    - Free tariffs
    - High limits that suit any user
    - Support for various nodes
    - Resource scaling
    - High processing speeds
- [**ZMOK**](https://zmok.io/)
  - [Docs](https://docs.zmok.io/)
  - Features
    - Front-running as a service
    - Global transactions mempool with search/filtering methods
    - Unlimited TX fee and infinite Gas for sending transactions
    - Fastest getting of the new block and reading of the blockchain
    - The best price per API call guarantee

## Further reading {#further-reading}

- [List of Ethereum node services](https://ethereumnodes.com/)

## Related topics {#related-topics}

- [Nodes and clients](/developers/docs/nodes-and-clients/)

## Related tutorials {#related-tutorials}

- [Getting started with Ethereum development using Alchemy](/developers/tutorials/getting-started-with-ethereum-development-using-alchemy/)
- [Guide to sending transactions using web3 and Alchemy](/developers/tutorials/sending-transactions-using-web3-and-alchemy/)
