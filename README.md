# ansible-squid-proxy

## Overview

This repository contains an Ansible playbook to set up a Squid proxy server with basic authentication.


## Setup

1. Clone the Repository to the server you wish to configure.

```sh
git clone https://github.com/eynsfordcq/ansible-squid-proxy.git
```

2. Install required packages

```sh
sudo apt update
sudo apt install -y python3-virtualenv 
```

3. Setup virtualenv 

```sh
python3 -m virtualenv --python="$(command -v python3)" .env &&
  source .env/bin/activate &&
  python3 -m pip install -U pip virtualenv &&
  python3 -m pip install -r requirements.txt
```

## Run

```sh
ansible-playbook playbook_squid_proxy.yaml
```