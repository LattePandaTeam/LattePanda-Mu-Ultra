# BIOS

This repository includes official releases and beta versions of BIOS for various branches, as well as related tools.

- ⚠ Generally, you should only upgrade the BIOS of the same branch. Cross-branch upgrades should only be performed when testing different BIOS features.
- ⚠ Upgrading the BIOS across different branches may invalidate the Secure Boot keys.
- ⚠ Upgrading to the incorrect BIOS branch may result in some functions of the carrier board not working properly.

------

## Naming Rule

**Format**
`SBCLNLCX[HW]-[Version].bin`

- **SBCLNLCX**: Platform identifier (LattePanda Mu Ultra 226V/256V)
- **[HW]**: 
    - PCBA Version
    - Initial Release Version: `R120`
- **[Version]**:`A`, `B`, `C`... (incremented alphabetically for each new release)

**Example**

`SBCLNLCXR120-A.bin`

------

## Folder Description

- **DFLT**: Default version BIOS, which is the BIOS branch that comes pre-installed on the LattePanda Mu Ultra compute module

------

## Release Timeline

```text
    2026-04
        │
        ●
        │
[Initial Release]
      DFLT
```

For specific model compatibility and functional changes, please refer to the `BIOS Release Notes` located in each branch's folder.
