# Simple REEF Node using Docker

This simple docker is meant to be used as a local dev node (no testnet or mainnet) for REEF chain, created following this guide: https://docs.reef.io/docs/developers/nodes/#start-a-local-development-node.

## Build image

```docker build -t reef-node-v10 .```

## Run node

```docker run -d --name=reef-node-v10 -dit -p 30333:30333 -p 9944:9944 -p 9933:9933 reef-node-v10```

## Attach log

```docker logs reef-node-v10 --follow```