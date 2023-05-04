# Traefik front auth proxy examples

This repository provides two examples of traefik used as a an authentification proxy delegating auth to a bundled keycloak.

## Usage

1. Check `.env.sample` file from each directory and use them to create your own `.env` file.
2. Deploy the stack with `docker compose up -d` (you might need to do it a few time as there is no proper waiting for keycloak to be available as the image does not come with `curl` or `wget` with installed)
3. Connect to keycloak
4. Create a client and note the `client-id` and `client-secret`

## Resources

- https://github.com/BlackBeltTechnology/traefik-keycloak-sso-reverse-proxy
- https://brianturchyn.net/traefik-forwardauth-support-with-keycloak/
- https://github.com/mesosphere/traefik-forward-auth

- https://github.com/oauth2-proxy/oauth2-proxy
- https://alex.thom.ae/2019/10/20/protect-website-oauth2_proxy-traefik/

