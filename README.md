<p align="center">
  <a href="https://github.com/ShaanCoding/ReadME-Generator">
    <img src="redash.png" alt="Logo" height="80">
  </a>

  <h3 align="center">Setup self-hosted Redash in windows</h3>

  <p align="center">
    An Awesome way to try and test redash on your local and do a POC for your team.
  </p>
</p>

## Table Of Contents

- [Table Of Contents](#table-of-contents)
- [About The Project](#about-the-project)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Authors](#authors)

## About The Project

This project aims to provide a comprehensive guide on setting up a local development environment for Redash, a popular open-source data visualization and dashboarding tool, on a Windows machine. Redash is typically hosted on Linux servers, but this guide focuses on enabling Windows users to easily test and develop with Redash without the need for a separate Linux server.

Developers and data analysts often need to test and develop Redash features, plugins, and customizations in a local environment before deploying to a production server. While Linux is the recommended platform for hosting Redash, this project aims to make it more accessible to Windows users for local testing and development.


## Getting Started

### Prerequisites

1. Ensure you have Windows 10 or later with [WSL](https://learn.microsoft.com/en-us/windows/wsl/install) installed and configured.
2. [Docker desktop](https://www.docker.com/products/docker-desktop/) with the default configuration using Linux containers.
3. [Git](https://git-scm.com/download/win)


### Installation

1. Clone the repo

```sh
git clone https://github.com/anujhsrsaini/redash.git
```

*You can change the environment variables if you want but there isn't much need for it.*

2. Run the below command to create a DB to store necessary information of Redash in PostgreSQL.

```sh
docker-compose run — rm server create_db
```

3. Run the docker container using the below command to run it in detached mode.

```sh
docker-compose up -d
```

4. Use the browser to navigate to localhost:5000 to setup redash initially.

5. Now, you can explore different functionalities of redash by setuping up different connections and building reports/dashboards.


## Authors

- **[Anuj Saini](https://www.linkedin.com/in/anuj-saini-7230a0257/)**