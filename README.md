# Example FastAPI using Sqllite DB 

## Deploy Guide
Use the supplied `Dockerfile` to build the image and deploy in any service that supports containers. Azure, AWS, GCP, etc.

This lets you run without any configuration changes.

## Local Development

### Build the Docker Image
Build the docker image using the following command 

```
docker build -t example-api .
```
__NOTE__: To build this locally you will need docker
### Run on a container

```
docker run -d --name mycontainer -p 80:80 example-api
```

## Libraries used in Creating the project

```commandline
pip install "fastapi[all]"

pip install "uvicorn[standard]"
```

// Thin layer on top of Pydantic and SQLAlchemy
```commandline
pip install sqlmodel
```

