## Usage

### First time server setup

```bash
$ ansible-playbook server_setup.yml --tags=setupping
```

### Setup only docker

```bash
$ ansible-playbook server_setup.yml --tags=setupping --skip-tags=app
```

### Setup only app

```bash
$ ansible-playbook server_setup.yml --tags=setupping --skip-tags=docker
```

### Update application

```bash
$ ansible-playbook update_app.yml --tags=updating
```
