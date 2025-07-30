# Tyk Pro Demo using Docker

## Quick start

### Prerequisites

1. Install [Docker](https://docs.docker.com/get-docker/)
2. Get a license for [Tyk Self-Managed](https://tyk.io/sign-up/) 


### Deploying Tyk

1. Clone the repo: 
```
git clone https://github.com/munkiat/tyk-poc && cd tyk-poc
```

2. Create a .env file with the below variables (see .env.example) 
```
DASH_LICENSE=<YOUR_LICENSE>
```

3. Run `docker-compose up`

```
---------------------------
Your Tyk Dashboard URL is http://localhost:3000

user: developer@tyk.io
pw: 1fty377f
---------------------------
Your Tyk Gateway URL is http://localhost:8080
---------------------------
Your Developer Portal URL is http://localhost:3001

user: portaladmin@tyk.io
pw: 1fty377f
---------------------------
```

### Cleanup Docker Containers

To delete all docker containers as well as remove all volumes from your host:

```
$ docker-compose down -v
```


