# Toolbox Collection for Cúram SPM

### Description

This collection includes helpful Ansible roles for installing prerequisite software and helper tools for building and testing Cúram Social Program Management.

### Installation

Install via Ansible Galaxy:

`ansible-galaxy collection install merative.spm_toolbox`

Or include this collection in your playbook's requirements.yml file:

```
---
collections:
  - name: merative.spm_toolbox
```

### Develop in VS Code dev container

You can use VS Code dev container in the project.

After container started, just run:

```
pip install -r requirements.txt
```

Then you can do molecule testing:

```
export ARTIFACTORY_URL=https://[your company or personal artifactory url]/artifactory
export ARTIFACTORY_REPO=software-installer-repo
export ARTIFACTORY_TOKEN=[token to your artifactory]
export LOCAL_PATH=/opt/spm-middleware
molecule test -s jfrog --destroy never
```

Happy Coding!
