# dbs-snapshot

`dbs-snapshot` is a fork of [Firecracker microvmm's](https://github.com/firecracker-microvm/firecracker) `snapshot` crate. It was done so because the Firecracker maintainers [have no plan to publish the crate on crates.io](https://github.com/firecracker-microvm/firecracker/issues/4162).

`dbs-snapshot` provides a version tolerant serialization and deserialization facilities and implements a persistent storage format for saving rust struct states. It can form a basis of many useful functionalities such as VM snapshot for rust-based VMMs, as well as user space program live upgrade for other projects like [Nydus](https://github.com/dragonflyoss/image-service/).

# Disclaimer

Please note that the crate is released from v1.5.0 because that is the initial Firecracker release version the crate was taken from.

We will use sematic versioning. The API backward-compatibilites will always be reserved across patch version updates. The backward-compatibilities across minor version updates will be preserved in a best effort manner. Whenever API backward-compatibility is broken on purpose, we will bump the major version.
