# Ignition

Ignition is the utility used by CoreOS Container Linux to manipulate disks during the initramfs. This includes partitioning disks, formatting partitions, writing files (regular files, systemd units, etc.), and configuring users. On first boot, Ignition reads its configuration from a source of truth (remote URL, network metadata service, hypervisor bridge, etc.) and applies the configuration.

Ignition has two main development branches: master and spec2x. This is the master branch which is for Ignition included in Red Hat CoreOS and Fedora CoreOS. For Ignition development for Container Linux see the [spec2x](https://github.com/coreos/ignition/tree/spec2x) branch.

## Usage

Odds are good that you don't want to invoke Ignition directly. In fact, it isn't even present in the Container Linux root filesystem. Take a look at the [Getting Started Guide][getting started] for details on providing Ignition with a runtime configuration.

## Contact

- Mailing list: [coreos-dev](https://groups.google.com/forum/#!forum/coreos-dev)
- IRC: #[coreos](irc://irc.freenode.org:6697/#coreos) on freenode.org
- Bugs: [issues][issues]

## Contributing

See [CONTRIBUTING](CONTRIBUTING.md) for details on submitting patches and the contribution workflow.

To help triage or fix bugs, see the current [Ignition issues](https://github.com/coreos/ignition/issues/).

## Reporting Bugs

- To report a bug, use the [bug tracker][issues]

## Config Validation

To validate a config for Ignition there are binaries for a cli tool called ignition-validate available [on the releases page][releases], and an online validator available [on the CoreOS website][online-validator].

[getting started]: doc/getting-started.md
[issues]:  https://github.com/coreos/ignition/issues/new/choose
[releases]: https://github.com/coreos/ignition/releases
[online-validator]: https://coreos.com/validate/
