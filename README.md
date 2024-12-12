# MLflow On-Premise Deployment using Docker Compose

Deploy an [MLFlow tracking server](https://mlflow.org/docs/latest/tracking/tutorials/remote-server.html) with Docker compose.

MinIO S3 is used as the artifact store and MySQL server is used as the backend store.

## Usage

Edit default credentials in [`./.env`](./.env) or published ports in [`./compose.yaml](./compose.yaml).

Start the tracking server with:

```bash
docker compose up -d --build
```

If running locally, access the MLFlow tracking server at its default port at [http://localhost:5000](http://localhost:5000).
