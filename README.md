# Try Blue/Green deployments with Traefik

Run
```shell
docker compose up -d
```

Open in your browser: http://docker.localhost/

You should be redirected to https://docker.localhost/ (you will probably need to accept the self issued certificate).

Open `./dynamic/dynamic.yml` and edit line 6

From `service: blue@file` to `service: green@file`

Refresh the browser and see the green service is routed to.

Voila, blue-green deployments!