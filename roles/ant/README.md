# ant

A role for installing Apache Ant

## Requirements

None

## Role Variables

| Property Name       | Default value                                         |
| ------------------- | ----------------------------------------------------- |
| `ant_version`       | `1.10.6`                                              |
| `ant_base_path`     | `[/opt | C:\Tools]`                                   |
| ------------------- | ----------------------------------------------------- |
| `profiled_path`     | `/opt/profile.d`                                      |

## Dependencies

A compatible JDK installed

## Example Playbook

```
---
- name: Install Ant 1.10.6
  hosts: all

  collections:
    - ibm.spm_toolbox

  pre_tasks:
    - name: Install JDK
      package:
        name: java-1.8.0-openjdk-devel

  roles:
    - ant

  vars:
    ant_version: "1.10.6"
    ant_base_path: "/opt"
```

## License

MIT
