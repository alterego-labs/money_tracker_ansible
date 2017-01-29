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

The following command will update application to the lastest version which is in the master branch, which is _HEAD_:

```bash
$ ansible-playbook update_app.yml --tags=updating
```

If you want to update application to the specific release number use the next command:

```bash
$ ansible-playbook update_app.yml --tags=updating -e money_tracker.git_version=v1.1.1
```
