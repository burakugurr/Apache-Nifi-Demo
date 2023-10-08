# Apache Nifi Example First Use

## Getting Started

With the robust data flow management capabilities offered by Apache NiFi, I have created a sample application and will guide you on harnessing the potential of this remarkable platform in the article below. If you're interested in delving deeper into NiFi, please refer to "What is Apache NiFi?" for a more comprehensive overview, which you can find in my article.

![image](https://github.com/burakugurr/Apache-Nifi-Demo/assets/42806395/403470aa-9e77-4e29-a3f3-f85326b5fe5b)

In the example application, we will transfer the incoming data to the database by making a request from the REST endpoint Nifi environment, which produces fake and random data. 

Endpoints will be:

1. https://random-data-api.com/api/v2/users

Article Adress:

1. https://medium.com/@burakugur/uçtan-uca-apache-nifi-uygulaması-3f2e04ced49e

2. https://medium.com/@burakugur/apache-nifi-nedir-f19111fb5802

## Requirements
- Docker

## Installation

### Run Nifi

```bash
docker run --name mynifi --network host -i -v ~/drivers/shared-directory:/opt/nifi/nifi-current/ls-target apache/nifi
```

### Run Postgres

```bash
docker run --name docker_postgres -e POSTGRES_PASSWORD=123456 -d -p 5432:5432 -v $HOME/docker/volumes/postgres:/var/lib/postgresql/data postgres
```

## License

This project is licensed under the MIT License. For more details, refer to the LICENSE file.



