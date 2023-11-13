[Doc](https://developer.concordium.software/en/mainnet/smart-contracts/guides/setup-tools.html)

Install rustup (installer for Rust, which installs both Rust and Cargo)
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
Use rustup to install the Wasm
```
rustup target add wasm32-unknown-unknown
```
Install cargo-concordium
~~~
 cargo install --locked cargo-concordium
~~~
~~~
cargo concordium --help
~~~
warning: spurious network error (1 tries remaining): [7] Couldn't connect to server (Failed to connect to index.crates.io port 443 after 0 ms: Couldn't connect to server)
error: failed to compile `cargo-concordium v3.1.4`, intermediate artifacts can be found at `/tmp/cargo-installjW7DcA`.
