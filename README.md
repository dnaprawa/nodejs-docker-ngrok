# NodeJS app with Docker & Ngrok integration

This repository contains an example of NodeJS app that can be publicly accessible over Internet with some simple steps using Docker and Ngrok.

## How to run

**Step 1. Getting Ngrok auth token**

* Create an account at https://dashboard.ngrok.com/signup

* Get auth token from https://dashboard.ngrok.com/get-started/your-authtoken and paste it to `ngrok.yml` file.

Example content of `ngrok.yml`
```yaml
authtoken: 25C37lPIJNplRM6EBUXWpgCNDbo_tuxgXQDrCfm7hgbP7MDJ
```

**Step 2. Clone the repository and type:**

```sh
docker-compose build
docker-compose up -d
```

After run, by default Ngrok UI will be available at http://localhost:4040 where you will find your public URL assigned by ngrok.


