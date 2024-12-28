
# Docker Build and Push Commands

## Java 8

```bash
docker build ./scala2.13-java8-ubuntu/.  -t eff3ct/spark:3.5.4-scala2.13-java8-ubuntu
docker tag eff3ct/spark:3.5.4-scala2.13-java8-ubuntu eff3ct/spark:latest
docker push eff3ct/spark:latest
docker push eff3ct/spark:3.5.4-scala2.13-java8-ubuntu
docker build ./scala2.13-java8-python3-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java8-python3-ubuntu
docker build ./scala2.13-java8-r-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java8-r-ubuntu
docker build ./scala2.13-java8-python3-r-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java8-python3-r-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java8-python3-r-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java8-python3-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java8-r-ubuntu
```

## Java 11

```bash
docker build ./scala2.13-java11-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java11-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java11-ubuntu
docker build ./scala2.13-java11-python3-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java11-python3-ubuntu
docker build ./scala2.13-java11-r-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java11-r-ubuntu
docker build ./scala2.13-java11-python3-r-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java11-python3-r-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java11-python3-r-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java11-python3-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java11-r-ubuntu
```

## Java 17

```bash
docker build ./scala2.13-java17-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java17-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java17-ubuntu
docker build ./scala2.13-java17-python3-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java17-python3-ubuntu
docker build ./scala2.13-java17-r-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java17-r-ubuntu
docker build ./scala2.13-java17-python3-r-ubuntu/. -t eff3ct/spark:3.5.4-scala2.13-java17-python3-r-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java17-python3-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java17-r-ubuntu
docker push eff3ct/spark:3.5.4-scala2.13-java17-python3-r-ubuntu
```
