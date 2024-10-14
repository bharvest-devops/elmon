# ELmon

`ELmon` is a monitoring tool designed specifically for Execution Layer Node operator on the Berachain. With `ELmon`, operators can effortlessly verify the health. Additionally, this tool promptly alerts operators in case any issues arise with nodes.

### Contents

- [ELmon](#ELmon)
  - [Monitoring List](#monitoring-list)
  - [Features](#features)
  - [Quick Guide](#quick-guide)

## Monitoring List

- Sync Status: Monitors whether the node is completely synced. Triggers an alarm if the node is still syncing.

- Block Height Increasing: Monitors the block height to ensure it's increasing. Triggers an alarm if the height is stuck for a certain period.

- Number of Peers: Monitors the number of peers connected. Triggers an alarm if the number of peers falls below a certain threshold.

- Number of Queued Transactions in Txpool: Monitors the number of queued transactions in the txpool. Triggers an alarm if the number of queued transactions exceeds a certain threshold.

## Features

- JSON API
  - Access monitoring results via a JSON API, available at the following path: `/`.
- Telegram Alerts
  - Receive alerts via Telegram if any issues arise with your node.

## Quick Guide

1. Build

```bash
go build
```

2. Configure `config.toml` file

```bash
cp config.toml.example config.toml
```

1. Run

```bash
./elmon
```
