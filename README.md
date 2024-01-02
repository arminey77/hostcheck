# HostCheck stage inventory

# Quick Start

> Note: Don't forget to replace `<YOUR_USER>` with your own.
```
git clone --recurse-submodules --remote-submodules <THIS_REPO_URL>
cd hostcheck
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
ansible-playbook -K -k -i ../inventory main.yml -b -e 'ansible_user=<YOUR_USER>@<ENV_DOMAIN>'
```

> Note: To see verbose, add `-v` to `ansible-playbook` command

# Notes
After HostCheck project update run this command:
```
git submodule update --recursive
or
git pull --recurse-submodules
```