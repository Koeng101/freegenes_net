
# The XYZ Network
By: Keoni Gandall, 2020-03-26

## Abstract

DNA distribution networks are inefficient, expensive, and inclusive. This hinders widespread collaboration and gatekeeps the bioeconomy to established players. We present a new kind of distribution network that leverages marginal costs of reproduction of biological materials and wide shipping networks. Widespread distribution of static biological materials allows for distributed verification and experimentation while drastically lowering costs for new people to enter the field. 

## Introduction

Currently, DNA material is mostly distributed through informal networks or centralized organizations. These informal networks are often highly dependent on who you know, while the centralized organizations are slow to adapt to changes in the field and have unintentionally created inefficient material monopolies.

The scope of the XYZ Network is small. The goal of the XYZ Network is to implement a method for widespread distribution of physical biological materials (such as plasmid DNA or strains), while remaining agnostic to form and annotation of those materials. 

There are 4 important parts of the XYZ Network:
- Blocks, which are unit of physical material distributed through the XYZ Network. 
  - For example, a 384-well plate of dried plasmid DNA could be a Block. 
  - Blocks which are identical to each other are part of a Block Group. Each Block Group has a finite number of Blocks that can be spread throughout the network.
- Hosts, which are organizations that can validate and optionally produce Blocks for the XYZ Network. 
  - Hosts are crucial in ensuring quality control within the network, and so must be willing to verify the integrity of Blocks. 
  - Hosts which create new Blocks distribute them throughout the Host network, where it is up to other Hosts whether or not those Blocks should be distributed downstream. For example, other Hosts could reject Blocks because they contain illegal genetic material.
- Relays, which are organizations that can distribute Blocks to Users in the XYZ Network. 
  - Hosts do not need to be Relays and Relays do not need to be Hosts. Hosts will often be Relays, but most Relays will be downstream from Hosts, simply receiving and forwarding Blocks throughout the network.
- Users, who are the people at the edges of the network that actually use the Blocks to do things.

The XYZ Network is designed to enable getting many Blocks into the hands of as many Users as possible, while ensuring that Blocks faithfully deliver their materials.

### Blocks

A XYZ Block is a physical object that is spread throughout the network. The most important thing about Blocks is that many *identical* Blocks are distributed throughout the XYZ Network at a time, which means those Block Groups can be independently verified as faithful. Once that group of Blocks is released into the network, it can never be released again: any reculture or recreation of material produces new Blocks, which must be verified once again.

A Block must be:

- Inseparable. If plates are the accepted form of a Block, 1 Plate == 1 Block, and 2 Plates == 2 Blocks.
- Independent. All information necessary to learn what a Block contains must be independent of any URLs or websites which may die and that information must be physically transfered with the Block.
- Isolated. A Block originates from one, and only one place. 

These rules are to make Blocks idempotent or stable from outside interference. As said above, groups of Blocks may only be released *once* into the network, and must all be *identical* to each other. Even if one plate is pinned in order to create 2 deep well plates, each of those deep well plates produce different Blocks, which must be independently verified.

### Hosts

A XYZ Host is an organization that shares responsibility in maintaining the integrity of the network. The network does not use true peer-to-peer distribution because the incredibly scalability of production and validation of DNA material in biotech. Hosts have 2 responsibilities:

- Verification of all Blocks passing through the network. Raw data from the verification must be publicly presented: pass/fail is not acceptable.
- Initiation of voting and voting to filter Blocks before they get distributed. A Host can initiate a vote to filter a Block for any reason, though Blocks should only be filtered for lawlessness and to prevent network spam. 

In exchange for providing these 2 services, Hosts get a couple advantages that Relays do not get:

- Opportunity to add new Blocks to the network. Any Host adding Blocks to the network must first independently verify their Block Group - Hosts may not use the network for cheap verification of new constructs.
- Ability to ask for certain number of Blocks per Block Group. Hosts producing new Blocks must deliver the desired number of Blocks to every other host. If that number is not delivered, Blocks risk being filtered before they are distributed.
- Early access. When Hosts receive new Blocks, they must wait before giving Blocks to Relays to allow for filtering.

When a Block Group is initialized on the network, it is first sent to the Hosts. After a short period of time, allowing for verification and filtering, the Blocks can be sent to Relays from Hosts. The exception to this rule is when a Relay is between two Hosts, in which case the Relay must be prepared to drop the Blocks it receives if the Hosts decide to filter the Block from the network.

The point of distributed verification of Blocks is that it institutes a kind of objective peer-review. Raw data is required so that the peers can both review and be reviewed.

### Relays

A XYZ Relay is an organization that forwards Blocks throughout the network. Relays have 3 responsibilities:

- Safe storage of all Blocks they receive.
- Maintenance of their Block inventory list, accessible to the public.
- Shipment of Blocks to Users.

Relays must get Blocks from Hosts. Although Relays cannot initiate new Blocks into the network, they can partner with Hosts to do so. 

Some Blocks will be in higher demand than other Blocks because of the materials they contain. Hosts who want as much distribution as possible will need to mint new Blocks with popular materials to respond to demand - this requires knowledge of what the Relays are shipping.

### Users

A XYZ User is any organization or person that gets Blocks. Users have 1 responsibility:

- To make the world a better place (without causing harm to others or the environment)
