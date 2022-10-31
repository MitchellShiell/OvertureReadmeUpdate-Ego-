# Ego - Authentication & Authorization 

<br />

<a href="https://www.overture.bio/"><img src="overture_logo.png" width="66%"></a>

<br />

[<img src="https://img.shields.io/badge/chat-on--slack-blue">](http://slack.overture.bio) 
[<img src="https://img.shields.io/badge/License-gpl--v3.0-blue">](https://github.com/overture-stack/ego/blob/develop/LICENSE)

## Worry Less Science More

We (the [OICR Genome Informatics Team](https://softeng.oicr.on.ca/team/)) develop the [Ego](https://www.overture.bio/products/ego/) authentication and authorization microservice in this Overture repository. 

[Overture]((https://www.overture.bio/)) is a collection of open-source, extendable solutions, designed for big-data genomic science. Our core products offer a comprehensive set of tools for securely contributing, accessing, analyzing, visualizing and sharing molecular and clinical data. Visit our [website](https://www.overture.bio/) for more information on what Overture has to offer, and check out our other projects on [GitHub](https://github.com/overture-stack/).

## Ego - Authentication & Authorization

<br />

<p align="center"><img alt="Ego in action" src="https://www.overture.bio/static/screenshot-21fc2cfc0ac1c3fd9bd7e62196477554.png"></p>

Access to sensitive and valuable information necessitates complex and secure user authentication and authorization methods. [Ego](https://www.overture.bio/products/ego/)  simplifies user management by providing a secure system to authenticate and authorize users of your application. 

[Ego](https://www.overture.bio/products/ego/) uses well-known single-sign-on identity providers like Google, GitHub, LinkedIn and ORCiD in place of managing usernames and passwords. 

Ego is [OAuth 2.0](https://oauth.net/2/) and [OpenID Connect](https://auth0.com/docs/authenticate/protocols/openid-connect-protocol) compliant. It is written in JAVA and uses [Sprint Boot](https://spring.io/projects/spring-boot) and [Spring Security Frameworks](https://spring.io/projects/spring-security). Because it uses [JSON Web Tokens (JWT)](https://jwt.io/) for stateless authorization, it can scale to accommodate many users. See our thorough [documentation](https://www.overture.bio/documentation/ego/) for further details. 

## Related Products 

<br />

<p align="left" ><img alt="Overture overview" src="https://www.overture.bio/static/124ca0fede460933c64fe4e50465b235/a6d66/system-diagram.png"></p>

While each component can be deployed independently within any given software architecture our core solutions can also work in concert to provide an end-to-end data management lifecycle. This data management system (DMS) is designed to meet the needs of modern large-scale genomic research. Please see our [DMS documentation](https://www.overture.bio/documentation/dms/) for more information on our data management system (DMS).



## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Contribution](#how-to-contribute)
- [Feedback](#feedback)
- [Code of Conduct](#code-of-conduct)
- [License](#license)

## Installation

For more information please see the documentation linked below:

- [Setup Prerequisites](https://www.overture.bio/documentation/ego/installation/prereq/)
- [Installation](https://www.overture.bio/documentation/ego/installation/installation/)
- [Configuration](https://www.overture.bio/documentation/ego/installation/configuration/)
- [Authentication](https://www.overture.bio/documentation/ego/installation/authentication/)



<!--

## Quick Start

 Here you will find a simplified quickstart guide to getting Ego setup. 

<br />

### 1. Set up a google oauth client app; 
- [summary steps linked here](https://www.overture.bio/documentation/ego/installation/prereq/#google). 
- Use the following redirect URI: ```http://localhost:8081/oauth/code/google```

<br />

### 2. Update  ```docker-compose-all.yml``` with the provided client id and secret 

```
spring.security.oauth2.client.registration.google.clientId : "<insert-provided-client-Id>"
spring.security.oauth2.client.registration.google.clientSecret: "<insert-provided-clientSecret>"
```

<br />

### 3. Run docker compose

```
docker-compose -f docker-compose-all.yml up 
```

You will need to wait for all the services to boot up, to watch the progress you can type the following into a seperate terminal

```
watch -n 2 docker service
```

<br />

### 4. Ego requires seed data to authorize the Ego UI as a client. 

```
docker exec ego_postgres_1  psql -h localhost -p 5432 -U postgres -d ego --command "INSERT INTO EGOAPPLICATION (name, clientId, clientSecret, redirectUri, description, status, errorredirecturi) VALUES ('ego ui', 'ego-ui', 'secret', 'http://localhost:8080/', '...', 'APPROVED', 'http://localhost:8080/error') on conflict do nothing"
```

Alternatively if you have ```Make``` installed you can run  ```make init-db```

### 5. Access the Ego UI through ```http://localhost:8080/ego-ui```
- This will require your google sign in 
- Once signed in you will have access to the admin dashboard (image above).
- The Ego swagger ui can be located at ```http://localhost:8080/swagger-ui.html```

<br />

-->

<!--
#### 1. Set up a database.
- Install [Postgres](https://www.postgresql.org/about/)
- Create a database

```
sudo -u postgress psql
create database ego;
q exit out of psql
```

<br />

### 2. Define the tables in your database.
- Copy the [psql.schema.spl](https://github.com/overture-stack/ego/blob/develop/src/main/resources/schemas/01-psql-schema.sql) file locally
- Execute the SQL script to setup the tables

```
psql -U postgres -d ego -a -f psql-schema.sql
```
<br />

### 3. Run one of the three supported Ego profiles
- ```Default``` is the most simple profile. It allows you to test API endpoints with a valid JWT
- ```Auth``` allows all the above as well as including JWT validations 
- ```Secure``` allows all the above as well as integration with https protocol



```
psql -U postgres -d ego -a -f psql-schema.sql
```

<br />

-->

## Usage

For more information please see the documentation linked below:

- [Using the Admin UI](https://www.overture.bio/documentation/ego/user-guide/admin-ui/)
- [Using the API](https://www.overture.bio/documentation/ego/user-guide/api/)


## Contribute

* [Making a Contribition ](CONTRIBUTING.md)
* [Filing an issue](https://github.com/overture-stack/ego/issues)

## Feedback

* Connect with us on [Slack](http://slack.overture.bio)
* [Upvote](https://github.com/overture-stack/ego/issues?q=is%3Aopen+is%3Aissue+label%3Anew-feature+sort%3Areactions-%2B1-desc) feature requests

## Code of Conduct

&emsp; [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)

## License

Licensed under the [GNU Lesser General Public License v3.0](LICENSE.txt) license.
