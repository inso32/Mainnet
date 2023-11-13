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
