# OpenIM Docker Usage Instructions 📘

> **Documentation Resources** 📚

- [Official Deployment Guide](https://docs.openim.io/guides/gettingstarted/dockercompose)

## :busts_in_silhouette: Community

- 💬 [Follow us on Twitter](https://twitter.com/founder_im63606)
- 🚀 [Join our Slack channel](https://join.slack.com/t/openimsdk/shared_invite/zt-22720d66b-o_FvKxMTGXtcnnnHiMqe9Q)
- :eyes: [Join our WeChat Group](https://openim-1253691595.cos.ap-nanjing.myqcloud.com/WechatIMG20.jpeg)

## Environment Preparation 🌍

- Install Docker with the Compose plugin or docker-compose on your server. For installation details, visit [Docker Compose Installation Guide](https://docs.docker.com/compose/install/linux/).

## Repository Cloning 🗂️

```bash
git clone https://github.com/openimsdk/openim-docker
```

## Configuration Modification 🔧

- Modify the `.env` file to configure the external IP. If using a domain name, Nginx configuration is required.

  ```plaintext
  # Set the external access address (IP or domain) for MinIO service
  MINIO_EXTERNAL_ADDRESS="http://external_ip:10005"
  ```

- For other configurations, please refer to the comments in the .env file

## Service Launch 🚀

- To start the service:

```bash
docker compose up -d
```

- To stop the service:

```bash
docker compose down
```

- To view logs:

```bash
docker logs -f openim-server
docker logs -f openim-chat
```

> ### Note:
>
> If you can't connect Docker Hub, you can use the following command:
>
> `docker compose -f docker-compose-cn.yaml up -d`

## Quick Experience ⚡

For a quick experience with OpenIM services, please visit the [Quick Test Server Guide](https://docs.openim.io/guides/gettingStarted/quickTestServer).
