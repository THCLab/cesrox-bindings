# Self-Addressing Identifier - WASM

WASM binding for [Rust SAID](https://github.com/THCLab/cesrox/tree/master/said)


### Prerequisites
`cargo install wasm-pack`

### Run
`wasm-pack build --target web`

Serve the root directory of the project with a local web server, (e.g. `python3 -m http.server`)
Load `index.html` from the web server (e.g. http://localhost:8000)
