# chrome

The `chrome` role downloads chrome and chromedriver appropriate for the OS.

## Requirements

None

## Role Variables

| Property Name     | Default value |
| ----------------- | ------------- |
| `chrome_owner`     | `root`        |
| `chrome_group`     | `root`        |

The chrome always use `$latest` version for Linux platforms to download the latest available binary.

## Dependencies

None

## Example Playbook

```
---
- name: Install Chrome
  hosts: all

  collections:
    - merative.spm_toolbox

  roles:
    - chrome

```

## License

MIT
