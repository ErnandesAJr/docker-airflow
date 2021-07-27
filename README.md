# Docker Airflow

## Resources

Min: 4Gb Mem RAM

## Initialize

### Create environment for python

Using [Anaconda](https://anaconda.org/conda-forge/awswrangler)

```bash
conda create --name airflow python=3.8
```

### Configure

```bash
echo -e "AIRFLOW_UID=$(id -u) \nAIRFLOW_GID=0" > .env
```

### Instance airflow using docker-compose

```bash
docker-compose up airflow-init
```

```bash
docker-compose up
```

### Acess

localhost:8080

user default = airflow
password default = airflow

### Command for verify Version

docker exec <id-container-airflow-docker_airflow-webserver_1> airflow version

## Download

https://airflow.apache.org/docs/apache-airflow/stable/docker-compose.yaml

curl -LfO 'http://apache-airflow-docs.s3-website.eu-central-1.amazonaws.com/docs/apache-airflow/latest/docker-compose.yaml'
