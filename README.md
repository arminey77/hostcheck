# HostCheck stage inventory

# Quick Start
```
git clone --recurse-submodules --remote-submodules https://gitops.asax.ir/platfrom-team/kubernetes-platform/kubernetes-infrastructure/observability/hostcheck-inventory-stage
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