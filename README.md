# Example using Ory Oathkeeper with cookie session authenticator

This example shows basic configuration of `cookie_session` authenticator for Ory Oathkeeper.

## Develop

Ory Oathkeeper Access Rules: [`access-rules.yml`](./oathkeeper/access-rules.yml) Ory Oathkeeper Configuration:
[`oathkeeper.yml`](./oathkeeper/oathkeeper.yml)

### Prerequisites

1. [Docker](https://docs.docker.com/get-docker/)
1. [Ory Oathkeeper](https://www.ory.sh/docs/oathkeeper/install)

### Run locally

```bash
git clone git@github.com:ory/examples
cd examples/oathkeeper/02-authenticators
docker-compose up
```

Wait for a couple of seconds and open `http://127.0.0.1:8080/hello`
