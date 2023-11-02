# nodejs

The `nodejs` role downloads NodeJS.

## Requirements

None

## Role Variables

| Property Name     | Default value |
| ----------------- | ------------- |
| `nodejs_version`  | `v18.12.0`    |
| `profiled_path`   | `/opt/profile.d` |

## Dependencies

None

## Example Playbook

```
---
- name: Install NodeJS
  hosts: all

  collections:
    - merative.spm_toolbox

  roles:
    - nodejs
```

## License

MIT
