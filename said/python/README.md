# Self-Addressing Indetifier - python

Python binding for [Rust SAID](https://github.com/THCLab/cesrox/tree/master/said)


## Build

    cargo build --release

Output `.so` file copied to directory with your code.

## Example (python3)

    from libsaid_python import Derivation, Sai
    data = "something to hash"
    print("Example of self adressing identifier of \"" + data + "\" using Blake3_256 derivation:")
    sai = Sai.derive(Derivation.Blake3_256, data)
    print(sai)
    assert Sai.verify(sai, data)
    assert not Sai.verify(sai, "something else")

