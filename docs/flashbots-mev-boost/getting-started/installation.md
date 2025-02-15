# Installation

`mev-boost` can run in any machine, as long as it is reachable by the beacon client. The default port is **18550**. The most common setup is to install it in the **same machine as the beacon client.**

## Dependencies

- [Go 1.18+](https://go.dev/doc/install)

## From source

Install mev-boost with `go install`:

```bash
go install github.com/flashbots/mev-boost@latest
mev-boost -help
```

Or clone the repository and build it:

```bash
git clone https://github.com/flashbots/mev-boost.git
cd mev-boost
make build

# Show the help
./mev-boost -help
```

## From Docker image

We maintain a mev-boost Docker image at [https://hub.docker.com/r/flashbots/mev-boost](https://hub.docker.com/r/flashbots/mev-boost)

- [Install Docker Engine](https://docs.docker.com/engine/install/)
- Pull & run the latest image:

## Consensus client configuration guides

```bash
docker pull flashbots/mev-boost:latest
docker run flashbots/mev-boost -help
```
|  | MEV-Boost Client Guides |
| --- | --- |
| Teku | [Guide](https://hackmd.io/@StefanBratanov/BkMlo1RO9)|
| Prysm | [Guide](https://hackmd.io/@prysmaticlabs/BJeinxFsq) |
| Lighthouse | [Guide](https://lighthouse-book.sigmaprime.io/builders.html#mev-and-lighthouse) |
| Lodestar | [Guide](https://github.com/ChainSafe/lodestar/blob/unstable/docs/usage/mev-integration.md) |
| Nimbus | [Guide](https://github.com/status-im/nimbus-eth2/pull/3883) |