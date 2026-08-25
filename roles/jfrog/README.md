# jfrog

The `jfrog` role downloads JFrog CLI appropriate for the OS. It installs both
the v1 `jfrog` executable and the v2 `jf` executable.

## Requirements

None

## Role Variables

| Property Name     | Default value |
| ----------------- | ------------- |
| `jfrog_version`   | `1.54.1`      |
| `jf_version`      | `2.109.0`     |
| `jfrog_owner`     | `root`        |
| `jfrog_group`     | `root`        |

The `jfrog_version` and `jf_version` variables may be set to `$latest` for
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
    jfrog_version: "$latest"
    jf_version: "$latest"
```

## License

MIT
