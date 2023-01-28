# General
FRZ Smart Chain client

Forked from Official Golang execution layer implementation of the Ethereum protocol with optimization of commission parameters.

[![API Reference](
https://camo.githubusercontent.com/915b7be44ada53c290eb157634330494ebe3e30a/68747470733a2f2f676f646f632e6f72672f6769746875622e636f6d2f676f6c616e672f6764646f3f7374617475732e737667
)](https://pkg.go.dev/github.com/ethereum/go-ethereum?tab=doc)
[![Go Report Card](https://goreportcard.com/badge/github.com/ethereum/go-ethereum)](https://goreportcard.com/report/github.com/ethereum/go-ethereum)
[![Travis](https://travis-ci.com/ethereum/go-ethereum.svg?branch=master)](https://travis-ci.com/ethereum/go-ethereum)
[![Discord](https://img.shields.io/badge/discord-join%20chat-blue.svg)](https://discord.gg/nthXNEv)

## Building the source

For prerequisites and detailed build instructions please read the [Installation Instructions](https://geth.ethereum.org/docs/getting-started/installing-geth).

Building `geth` requires both a Go (version 1.18 or later) and a C compiler. You can install
them using your favourite package manager. Once the dependencies are installed, run

```shell
make geth
```

or, to build the full suite of utilities:

```shell
make all
```

## Run public node

Get your genesis file & boot key from FRZ Chain dev team

Then, make datadir folder

```shell
<PATH TO THE PROJECT FOLDER>/build/bin/geth --datadir <PATH TO DATADIR> init <GENESIS FILE>
```

Start builded client with such minimum parameters:

```shell
<PATH TO THE PROJECT FOLDER>/build/bin/geth --networkid 1995 --datadir=<PATH TO DATADIR> --bootnodes enode://<BOOTKEY>@publicnodes.frzchain.com:0?discport=4000 <YOUR RPC PARAMS>
```
