# `nico-admin-cli redfish lockdown-bmc-disable`

*[Hardware commands](../../hardware.md) › [redfish](./redfish.md) › **lockdown-bmc-disable***

## NAME

nico-admin-cli-redfish-lockdown-bmc-disable - Disable BMC lockdown
without applying the full host unlock policy

## SYNOPSIS

```text
nico-admin-cli redfish lockdown-bmc-disable [--extended]
[--sort-by] [-h|--help]
```

## DESCRIPTION

Disable BMC lockdown without applying the full host unlock policy

On Lenovo, disables firmware and BIOS settings lockdown while preserving
UEFIVariablesRO and legacy controls. Does not reboot the host.

## OPTIONS

`--extended`

Extended result output.

This is used by measured boot, where basic output contains just what you
probably care about, and "extended" output also dumps out all the
internal UUIDs that are used to associate instances.

`--sort-by <SORT_BY> [default: primary-id]`

Sort output by specified field

*Possible values:*

- primary-id: Sort by the primary ID

- state: Sort by state

`-h, --help`

Print help (see a summary with -h)

## Examples

```sh
nico-admin-cli redfish --address 192.0.2.10 --username admin --password mypassword lockdown-bmc-disable
```

---

**Related:** [Hardware commands](../../hardware.md) · [CLI reference index](../../README.md)
