# `time-server`

A simple time server written in Rust, which you can use to ensure your clients' clocks are in sync with a server.

## Setup and Usage

### Pre-requisites

- Rust & Cargo (https://doc.rust-lang.org/cargo/getting-started/installation.html)

### Running the server

1. Clone the repo
   ```bash
   git clone https://github.com/filiptronicek/time-server-rust.git
   ```
2. Run the server
   ```bash
   cd server
   cargo run
   ```
3. The server will be running on port 8000

### `clock-check` CLI

The `clock-check` CLI is a simple tool that you can use to consume and use the data from the time server. More info in its [README](./cli/README.md).

## Public instances

These are some public instances of the time server, which you can use to test from the CLI. To use one of these, supply the URL as the `--server` argument to the CLI. If you decide to host one yourself, please add it to this list.

| URL                                            | Description                                                                                                           |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| https://time.filiptronicek.workers.dev/        | A compatible time server hosted on Cloudflare Workers, which is based on the Javascript implementation of the server. |
| https://time-server.filiptronicek.workers.dev/ | A lightweight version of the server running on Cloudflare Workers with WebAssembly.                                   |

