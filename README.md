# blockfolio-api

[![bitHound Overall Score](https://www.bithound.io/github/bob6664569/blockfolio-api/badges/score.svg)](https://www.bithound.io/github/bob6664569/blockfolio-api) [![bitHound Dependencies](https://www.bithound.io/github/bob6664569/blockfolio-api/badges/dependencies.svg)](https://www.bithound.io/github/bob6664569/blockfolio-api/master/dependencies/npm) [![bitHound Code](https://www.bithound.io/github/bob6664569/blockfolio-api/badges/code.svg)](https://www.bithound.io/github/bob6664569/blockfolio-api)

[![Faire un don en Bitcoin](https://fr.cryptobadges.io/badge/micro/1LhMTZWBnRq6NTwWegYKdMUAiH9LrWEvyd)](https://fr.cryptobadges.io/donate/1LhMTZWBnRq6NTwWegYKdMUAiH9LrWEvyd)

Non-official Node.JS API Client for Blockfolio

Install
--
```sh
npm install blockfolio-api --save
```

Usage
--
```javascript
const BlockfolioAPI = require("blockfolio-api");

// BLOCKFOLIO_DEVICE_TOKEN is found under the "Settings" part of the app, in the bottom of the page
// The currency specified on second parameter is optional (default to "usd")
const Blockfolio = new BlockFolioAPI("BLOCKFOLIO_DEVICE_TOKEN", "eur");

Blockfolio.getPositions((err, positions) => {

    if (err) throw(err);

    console.log(positions);
});
```
