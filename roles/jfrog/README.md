# jfrog

The `jfrog` role downloads JFrog CLI appropriate for the OS.

## Requirements

None

## Role Variables

| Property Name     | Default value |
| ----------------- | ------------- |
| `jfrog_version`   | `1.39.5`      |
| `jfrog_owner`     | `root`        |
| `jfrog_group`     | `root`        |

The `jfrog_version` variable may be set to `$latest` for Linux platforms to download the latest available binary.

## Dependencies

None

## Example Playbook

```
---
- name: Install JFrog CLI
  hosts: all

  collections:
    - ibm.spm_toolbox

  roles:
    - jfrog

  vars:
    jfrog_version: "$latest"
```

## License

MIT
