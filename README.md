# HostCheck stage inventory

# Quick Start

> Note: Don't forget to replace `<YOUR_USER>` with your own.
```
git clone --recurse-submodules --remote-submodules https://gitops.asax.ir/platfrom-team/kubernetes-platform/kubernetes-infrastructure/observability/hostcheck-inventory-stage -e 'ansible_user=<YOUR_USER>@stdc.local' -e 'become_user=<YOUR_USER>@stdc.local'
cd hostcheck
python -m venv .venv
pip install -r requirements.txt
source .venv/bin/activate
ansible-playbook -K  -i ../inventory/stage/inventory.yml main.yml -b
```

> Note: To see verbose, add `-v` to `ansible-playbook` command

# Notes
After HostCheck project update run this command:
```
git submodule update --recursive
or
git pull --recurse-submodules
```