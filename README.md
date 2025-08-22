# Ruachnet Governance Blockchain Comunity - Based on Besu Ethereum Client 
 [![View Project Document](https://docs.google.com/document/d/1AJdiE0uOVFbBSLY-F_WLsKUa6k1yXvi9Y0r3wFJS7mI/preview)
 [![CircleCI](https://circleci.com/gh/hyperledger/besu/tree/main.svg?style=svg)](https://circleci.com/gh/hyperledger/besu/tree/main)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/3174/badge)](https://bestpractices.coreinfrastructure.org/projects/3174)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Ruachnet/project-ruachnet/blob/main/LICENSE)
 [![Discord](https://img.shields.io/discord/905194001349627914?logo=Hyperledger&style=plastic)](https://discord.gg/Mjup2t8G)
 [![Follow on X](https://img.shields.io/twitter/follow/RuachNet254)](https://twitter.com/RuachNet254)

Besu is an Apache 2.0 licensed, MainNet compatible, Ethereum client written in Java.

## Useful Links

* [Besu User Documentation](https://docs.google.com/document/d/1AJdiE0uOVFbBSLY-F_WLsKUa6k1yXvi9Y0r3wFJS7mI/preview)

## Docker
```bash
docker build -t besu-hgbc -f docker/Dockerfile .
```

## Testing the network
### Request Rpc version
```bash
curl -X POST https://rpc.anarchtech.dantalion.org -H "Content-Type: application/json" --data '{"jsonrpc":"2.0","method":"eth_blockNumber","params":[],"id":1}'
```
### Response
```json
{"jsonrpc":"2.0","id":1,"result":"0x0"}
```

## Other network tests
### Get chain ID
```bash
curl -X POST https://rpc.anarchtech.dantalion.org -H "Content-Type: application/json" --data '{"jsonrpc":"2.0","method":"eth_chainId","params":[],"id":1}'
```

### Get syncing status
```bash
curl -X POST https://rpc.anarchtech.dantalion.org -H "Content-Type: application/json" --data '{"jsonrpc":"2.0","method":"eth_syncing","params":[],"id":1}'
```

### Test peer to peer using web3 library
```js
const Web3 = require("web3");
const web3 = new Web3("https://rpc.anarchtech.dantaion.org");

(async () => {
  const block = await web3.eth.getBlockNumber();
  console.log("Current block:", block);
})();
```

### Test peer to peer using telnet
```bash
telnet 157.230.72.6 30303
```

### Test peer to peer using web3 library
```bash
nc -vz 157.230.72.6 30303
```

## Issues 

Besu issues are tracked [in the github issues tab][https://github.com/bdigismat/besu-hgbc].
See our [guidelines](https://lf-hyperledger.atlassian.net/wiki/spaces/BESU/pages/22154243/Issues) for more details on searching and creating issues.

If you have any questions, queries or comments, [Besu channel on Discord] is the place to find us.


## Besu Users

To install the Besu binary, follow [these instructions](https://besu.hyperledger.org/public-networks/get-started/install/binary-distribution).    

## Besu Developers

* [Contributing Guidelines]
* [Coding Conventions](https://lf-hyperledger.atlassian.net/wiki/spaces/BESU/pages/22154259/Coding+Conventions)
* [Command Line Interface (CLI) Style Guide](https://lf-hyperledger.atlassian.net/wiki/spaces/BESU/pages/22154260/Besu+CLI+Style+Guide)
* [Besu User Documentation] for running and using Besu


### Development

Instructions for how to get started with developing on the Besu codebase. Please also read the
[wiki](https://lf-hyperledger.atlassian.net/wiki/spaces/BESU/pages/22154251/Pull+Requests) for more details on how to submit a pull request (PR).  

* [Checking Out and Building](https://lf-hyperledger.atlassian.net/wiki/spaces/BESU/pages/22154264/Building+from+source)
* [Code Coverage](https://lf-hyperledger.atlassian.net/wiki/spaces/BESU/pages/22154288/Code+coverage)
* [Logging](https://lf-hyperledger.atlassian.net/wiki/spaces/BESU/pages/22154291/Logging) or the [Documentation's Logging section](https://besu.hyperledger.org/public-networks/how-to/monitor/logging)

### Profiling Besu

Besu supports performance profiling using [Async Profiler](https://github.com/async-profiler/async-profiler), a low-overhead sampling profiler.  
You can find setup and usage instructions in the [Profiling Guide](docs/PROFILING.md).

Profiling can help identify performance bottlenecks in block processing, transaction validation, and EVM execution.  
Please ensure the profiler is run as the same user that started the Besu process.

## Release Notes

[Release Notes](CHANGELOG.md)

## Reference Tests and JSON Tracing

Besu includes support for running Ethereum reference tests and generating detailed EVM execution traces.

To learn how to run the tests and enable opcode-level JSON tracing for debugging and correctness verification, see the [Reference Test Execution and Tracing Guide](REFERENCE_TESTS.md).

[Besu Issues]: https://github.com/bdigismat/besu-hgbc/issues
[Besu User Documentation]: https://docs.google.com/document/d/1AJdiE0uOVFbBSLY-F_WLsKUa6k1yXvi9Y0r3wFJS7mI/preview
[Besu channel on Discord]: https://discord.gg/Mjup2t8G
[Contributing Guidelines]: CONTRIBUTING.md
