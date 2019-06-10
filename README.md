# Node runtime types for `ink!`

Defines types for [ink!](https://github.com/paritytech/ink) smart contracts targeting [Substrate's `node-runtime`](https://github.com/paritytech/substrate/blob/master/node/runtime/src/lib.rs).

Supplies an implementation of the ink `EnvTypes` trait:

```
pub trait EnvTypes {
    /// The type of an address.
    type AccountId: parity_codec::Codec + PartialEq + Eq;
    /// The type of balances.
    type Balance: parity_codec::Codec;
    /// The type of hash.
    type Hash: parity_codec::Codec;
    /// The type of timestamps.
    type Moment: parity_codec::Codec;
}
```

See `ink!` [example](https://github.com/paritytech/ink/tree/master/examples/lang/erc20) for usage.

