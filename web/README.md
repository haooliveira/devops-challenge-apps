# Devops Web App


## Observation

You can ignore this `docker-compose.yml`. It's only a start point.

### install the node packages in the web container:
```sh
→ docker-compose run web npm install
```
> Docker will download all of the images for the container.

### start up the app:
```sh
→ docker-compose up
```

###  NOTE this app uses two env variables:

- PORT: the listening PORT
- API_HOST: the full url to call the API app. An example `http://web-api-host:port`

These two variables need to be set with docker-compose (WEB_PORT, API_HOST).
