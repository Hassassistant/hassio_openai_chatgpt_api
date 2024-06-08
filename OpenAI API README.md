ssh into Home Assistant and run the following commands:

```bash
sudo su -s /bin/bash
```

```bash
docker ps
```

#Get the Id of the HomeAssistant Container from the docker ps command

```bash
docker exec -it {Your Container ID} /bin/bash
```

```bash
source /config/.venv/bin/activate
```

Your prompt should look like this: 

(.venv) homeassistant:/config#

If not try:

```bash
source /srv/homeassistant/bin/activate
```
If you can't activate the environmnet run the remaining commands without the environment active:

```bash
pip install openai --upgrade
```

```bash
deactivate
```

```bash
exit
```