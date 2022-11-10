## OpenSea NFT Template

With the new [OpenSea royalty policies](https://twitter.com/opensea/status/1590466349683576832), it may be necessary for new NFT contracts to implement a marketplace filtering solution. The template in this repo
utilizes the [OpenSea operator-filterer library](https://github.com/ProjectOpenSea/operator-filter-registry) which allows contract owners to register
a list of blocked operators.

This repo includes templates for both OpenZeppelin's ERC721 and Chiru-Labs' ERC721A implementations. Both sample templates
use a blank blacklist to start (the `address(0)` parameter in the constructor). If you would like to use OpenSea's default list, you can either
import their DefaultOperatorFilterer or pass in `address(0x3cc6CddA760b79bAfa08dF41ECFA224f810dCeB6)` into the constructor.

To use this template, you can fork/clone the repo and run the `forge install` command.
