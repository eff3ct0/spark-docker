# Apache Spark Official Dockerfiles

## What is Apache Spark?

Spark is a unified analytics engine for large-scale data processing. It provides
high-level APIs in Scala, Java, Python, and R, and an optimized engine that
supports general computation graphs for data analysis. It also supports a
rich set of higher-level tools including Spark SQL for SQL and DataFrames,
pandas API on Spark for pandas workloads, MLlib for machine learning, GraphX for graph processing,
and Structured Streaming for stream processing.

https://spark.apache.org/

## Why this Apache Spark Docker Image?

The Apache Spark Docker image is a lightweight and easy-to-use Docker image for running Apache Spark on your system.

Because Apache Spark doesn't provide a Docker image with Scala 2.13 support, we created this Docker image to easily run Apache Spark with Scala 2.13.

## Features

- Scala 2.13 support
- Java 11 support / Java 17 support
- Python 3.10 support
- R 4.2 support

## Supported Tags and Dockerfiles

The following tags are available for this Docker image:

- `latest` (3.5.4-scala2.13-java11-python3-r-ubuntu)
- `3.5.4-scala2.13-java11-python3-r-ubuntu`, `3.5.4-scala2.13-java11-python3-ubuntu`, `3.5.4-scala2.13-java11-r-ubuntu`, `3.5.4-scala2.13-java11-ubuntu`
- `3.5.4-scala2.13-java17-python3-r-ubuntu`, `3.5.4-scala2.13-java17-python3-ubuntu`, `3.5.4-scala2.13-java17-r-ubuntu`, `3.5.4-scala2.13-java17-ubuntu`

For more information about the available tags and their corresponding Dockerfiles, please refer to the [tags](https://hub.docker.com/repository/docker/eff3ct/spark/tags) page.

## Getting Started

To use this Docker image, you'll need Docker installed on your system. Follow these steps to get started:

### Pull the Docker Image

Download the image from the Docker registry:

```bash
docker pull eff3ct/spark:latest
```

### Run the Docker Image

Run the Docker image:

```bash
docker run -it eff3ct/spark:latest /bin/bash
```

This will start a new container with the Spark image running. You can now use the Spark CLI to interact with the container.

## Usage

You can use the Spark CLI to interact with the container. For example, to run a Spark shell:

```bash
docker run --rm -it \
  -v /path/to/your/app:/app \
  eff3ct/spark:latest \
  /bin/bash -c "$SPARK_HOME/bin/spark-submit --class <YourMainClass> /app/your-spark-app.jar <args>"
```

This will start a new container with the Spark image running and open a Spark shell.

## License

This project is licensed under the [Apache License, Version 2.0](LICENSE).
