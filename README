## Overview

This is a simple seed project for running Nginx servers with TLS on hosts that have been provisioned with certificates and keys via Let's Encrypt. It assumes that certificates and keys have already been generated and that both `docker` and `docker-compose` are installed on the host.

## Prerequisites

* A server provisioned with `certbot`, `docker`, and `docker-compose`
* `certbot certonly` has been run on the server (e.g., the path `/etc/letsencrypt/live/<your-domain-name>/` exists)

## Setup

1. Clone this repo in a local directory (e.g., `/usr/local/src`)
2. Open `/<path-to-repo>/.env` and change the value for `LETSENCRYPT_FQDN` to your domain name
3. Run `docker-compose up -d`

Assuming that `docker-compose` starts the `web` service without issue, verify by navigating to `http://<your-domain-name>`. The client should be redirected to the server listening at `:443` and display a valid TLS certificate.