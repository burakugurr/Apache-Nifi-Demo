# Apache Nifi Example First Use

## Getting Started

Thanks to Apache NiFi's powerful data flow management capabilities, I have developed a sample application and will show you how to use this impressive platform in the article below. If you want to get more detailed information about Nifi, see What is Apache Nifi? You can read my article.

![image](https://github.com/burakugurr/Apache-Nifi-Demo/assets/42806395/11bdfd1b-385b-4bf0-bc0d-bae3144104b7)

In the example application, we will transfer the incoming data to the database by making a request from the REST endpoint Nifi environment, which produces fake and random data. 

Endpoints will be:

1. https://random-data-api.com/api/v2/users

Article Adress:

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



