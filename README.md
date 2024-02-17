# GitHub Runner Ansible

Ansible playbook that sets up your github runner given some config

## How to use
1. Edit `hosts.ini` file and add your gitlab runner's IP or if you have an SSH alias for it you can use that instead
2. Change the variables in the `hosts.ini` file to match yours
3. Your token can be found by heading to your repo URL, for example, https://github.com/hedche/ansible-github-runner, then `Settings` -> `Actions` -> `Runners` -> `New self-hosted runner`. The token will be in a section that looks like this (in this case the token is `APP3GJGWNJGNRWKLFJGNEGH3C`):
##### Configure
```
# Create the runner and start the configuration experience
$ ./config.sh --url https://github.com/hedche/ansible-github-runner --token APP3GJGWNJGNRWKLFJGNEGH3C
# Last step, run it!
$ ./run.sh
```
