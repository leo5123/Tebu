# Tebu

Discord chat based game!

*Made by [leo5123](https://github.com/leo5123) and [RyanQueirozS](https://github.com/RyanQueirozS).*

## Tech

- Skaffold
- Kubernetes
- Docker
- Helm
- Golang
 
## General information
This project is a **original** Discord bot that is also a game.

## Game content

- Combat system
- Item crafting
- Material gathering
- Exploration
- Lore
- Save

# Setup
You're going to need a running kubernetes cluster, if you dont have one execute ./l8ks up.

In case you don't have helm installed: 
https://helm.sh/docs/intro/install/
```
git clone https://github.com/jumbo-dog/Tebu.git
cd Tebu/
helm install operations -f ../kubernetes-secrets/myvalues.yaml ./charts/bot-service-chart/
```


Secrets yaml format
```
botServiceSettings:
  botToken: ""
  appId: ""
  databasePassword: ""
  databaseLogin: ""
image:
  tag: latest 
```

