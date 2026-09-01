# jfrog

The `jfrog` role downloads JFrog CLI appropriate for the OS. It installs
the v2 `jf` executable.

## Requirements

None

## Role Variables

| Property Name     | Default value |
| ----------------- | ------------- |
| `jf_version`      | `2.122.0`     |
| `jfrog_owner`     | `root`        |
| `jfrog_group`     | `root`        |

The `jf_version` variable may be set to `$latest` for
Linux platforms to download the latest available binary.

## Dependencies

None

## Example Playbook

```
---
- name: Install JFrog CLI
  hosts: all

  collections:
    - merative.spm_toolbox

  roles:
    - jfrog

  vars:
    jf_version: "$latest"
```

## License

MIT
