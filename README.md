
# The FreeGenes Network
By: Keoni Gandall, 2020-03-26

## Abstract

DNA distribution networks are inefficient, expensive, and inclusive. This makes hinders widespread collaboration and gatekeeps the synthetic biology community. We present a new kind of distribution network that leverages marginal costs of reproduction of biological materials and wide shipping networks. Widespread distribution of static biological materials allows for distributed validation and experimentation while drastically lowering costs for new people to enter the field. 

## Overview

Currently, DNA material is mostly distributed through informal networks or centralized organizations. These informal networks are often highly dependent on "who you know", while the centralized organizations are slow to adapt to changes in the field and have unintentionally created material monopolies.

The scope of the FreeGenes Network is small. The goal of the FreeGenes Network is to implement a method for widespread distribution of physical biological materials (such as plasmid DNA or strains), while remaining agnostic to form of distribution and annotation of those materials. 

There are 4 important parts of the FreeGenes Network:
- Blocks, which are unit of physical material distributed through the FreeGenes Network. For example, a 384-well plate of dried plasmid DNA could be a block. Blocks which are identical to each other are part of a Block Group. Each Block Group has a finite number of Blocks that can be spread throughout the network.
- Hosts, which are organizations that can validate and optionally produce Blocks for the FreeGenes Network. Hosts are crucial in ensuring quality control within the network, and so must be willing to verify the integrity of blocks. Hosts which create new Blocks distribute them throughout the network, where it is up to other Hosts whether or not those Blocks should be distributed downstream. For example, other Hosts could reject Blocks because they contain illegal genetic material.
- Distributors, which are organizations that can distribute Blocks for the FreeGenes Network. Hosts do not need to be Distributors and Distributors do not need to be Hosts. Hosts will often be Distributors, but most Distributors will be downstream from Hosts, simply receiving and forwarding Blocks throughout the network.
- Users, who are the people at the edges of the network that actually use the Blocks to do things.

The FreeGenes Network is designed to get as many Blocks into the hands of as many Users as possible, while ensuring that Blocks faithfully deliver their materials.

## Blocks

A FreeGenes Block is a physical object that is spread throughout the network. The most important thing about Blocks is that many *identical* Blocks are distributed throughout the FreeGenes Network at a time, which means those Block Groups can be independently verified as faithful. Once that group of Blocks is released into the network, it can never be released again: any reculture or recreation of material produces new Blocks, which must be verified once again.

A Block must be:

- Inseparable. If plates are the accepted form of Block, 1 Plate == 1 Block, and 2 Plates == 2 Blocks
- Independent. All information necessary to learn what a Block contains must be independent of any URLs or websites which may die and that information must be physically transfered with the Block.
- Isolated. A Block originates from one, and only one place. 

These rules are to make blocks idempotent or stable from outside interference. As said above, groups of Blocks may only be released *once* into the network, and must all be *identical* to each other. Even if one plate is pinned in order to create 2 deep well plates, each of those deep well plates produce different Blocks, which must be independently verified.

## Hosts



## Distributors


