# `nico-admin-cli redfish lockdown-bmc-enable`

*[Hardware commands](../../hardware.md) › [redfish](./redfish.md) › **lockdown-bmc-enable***

## NAME

nico-admin-cli-redfish-lockdown-bmc-enable - Enable BMC lockdown without
applying the full host lockdown policy

## SYNOPSIS

```text
nico-admin-cli redfish lockdown-bmc-enable [--extended]
[--sort-by] [-h|--help]
```

## DESCRIPTION

Enable BMC lockdown without applying the full host lockdown policy

On Lenovo, enables firmware and BIOS settings lockdown while preserving
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
nico-admin-cli redfish --address 192.0.2.10 --username admin --password mypassword lockdown-bmc-enable
```

---

**Related:** [Hardware commands](../../hardware.md) · [CLI reference index](../../README.md)
