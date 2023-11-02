# openjdk

The `openjdk` role downloads OpenJDK 8.

## Requirements

None

## Role Variables

None

## Dependencies

None

## Example Playbook

```
---
- name: Install OS openjdk-devel package
  hosts: all

  collections:
    - merative.spm_toolbox

  roles:
    - openjdk
```

## License

MIT
