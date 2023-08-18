- `[tendermint-proto]` Align the return signature of the `encode_vec` and
  `encode_length_delimited_vec` methods in the `Protobuf` trait with
  `prost::Message` by directly returning `Vec<u8>`.
  ([\#1323](https://github.com/informalsystems/tendermint-rs/issues/1323))
  * Remove mandatory cloning in `Protobuf` methods and let callers decide on
    clone beforehand for original value access
