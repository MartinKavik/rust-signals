## NEXT
* Fixing bug with `SignalExt::switch_signal_vec`.
* Adding in `SignalExt::map_value_signal` method.

## 0.3.31 - (2022-09-10)
* Adding in serde `Serialize` and `Deserialize` for `MapDiff`.
* Adding in `SignalExt::sample_stream_cloned` method.

## 0.3.30 - (2022-07-24)
* Adding in serde `Serialize` and `Deserialize` for `VecDiff`.

## 0.3.29 - (2022-07-15)
* Adding in `SignalVecExt::chain` method for concatenating two `SignalVec`.

## 0.3.28 - (2022-05-15)
* Adding in `apply_vec_diff` method to `MutableVec`.

## 0.3.27 - (2022-05-10)
* Adding in `option` and `result` functions.

## 0.3.26 - (2022-05-10)
* Introducing a `debug` feature to make the [`log` crate](https://crates.io/crates/log) optional.
* Adding in `SignalVecExt::debug` method which prints each `VecDiff` change to the console.

## 0.3.25 - (2022-04-18)
* The `signals::channel` implementation is now lock-free (if the allocator is lock-free).
* `Broadcaster` now impls `Clone`.
* `MutableVec` now impls `Clone`.
* `MutableBTreeMap` now impls `Clone`.
* Adding in `BoxSignal` and `LocalBoxSignal` type aliases.
* Adding in `BoxSignalVec` and `LocalBoxSignalVec` type aliases.
* Adding in `BoxSignalMap` and `LocalBoxSignalMap` type aliases.

## 0.3.24 - (2021-12-29)
* Changing `SignalExt::debug` to use the [`log` crate](https://crates.io/crates/log).
* Adding in new `signal_vec::from_stream` function.

## 0.3.23 - (2021-10-20)
* `Mutable::clone` is now lock-free.
* Adding in `SignalExt::debug` method which prints the state of the signal to the console.
* Fixing bug with `from_stream` function.

## 0.3.22 - (2021-06-13)
* Adding in `SignalExt::boxed` and `SignalExt::boxed_local` methods, for feature-parity with `FutureExt` and `StreamExt`.
* Adding in `Broadcaster::signal_ref` method.
* Fixing various bugs with `Broadcaster`.
