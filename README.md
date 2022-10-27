<!--Modeled from: "https://github.com/microsoft/vscode"-->
<!--Modeled from: "https://coding-boot-camp.github.io/full-stack/githubprofessional-readme-guide"-->


# Ego

[<img src="https://img.shields.io/badge/chat-on%20slack-blue">](http://slack.overture.bio)

This Overture repository is where we, the [OICR Genome Informatics Team](https://softeng.oicr.on.ca/team/), develop the Ego authentication & authorization microservice. Overture is a collection of open-source, extendable solutions for big-data genomic science. <!--Optional: Not only do we work on code issues here, we also publish our ... roadmap ... plans.--> Our source code is available to the general public under the [gpl-v3.0](LICENSE.txt) license.

<!--![](https://www.overture.bio/static/124ca0fede460933c64fe4e50465b235/a6d66/system-diagram.png)-->

## Description

<!--Provide a short description explaining the what, why, and how of your project. Use the following questions as a guide:-->

Ego is an [OAuth 2.0](https://oauth.net/2/) and [OpenID Connect](https://auth0.com/docs/authenticate/protocols/openid-connect-protocol) compliant application that simplifies user management by providing methods to authenticate and authorize users of your application through well-known social Single-Sign-On identity providers. Ego does not manage usernames and passwords, but instead relies on popular identity providers to complete this. Supported Single-Sign-On Identity providers include Google, GitHub, LinkedIn and ORCiD. Ego is written in JAVA and uses Sprint Boot and Spring Security Frameworks. It provides stateless authorization using [JSON Web Tokens (JWT)](https://jwt.io/) allowing it to scale very well to a large number of users. 

![](https://www.overture.bio/static/screenshot-21fc2cfc0ac1c3fd9bd7e62196477554.png)

<!--What the motivation to create ego?-->

<!--Why did you build this project?-->

<!--What problem does it solve?-->

<!--How does it solve this problem-->


---
<br />


## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Contribution](#how-to-contribute)
- [Feedback](#feedback)
- [Code of Conduct](#code-of-conduct)
- [License](#license)

## Installation 

For detailed instructions visit the [Overture Ego Installation guide](https://www.overture.bio/documentation/ego/installation/installation/).

## Usage

Instructions and examples for use. 

```
Include screenshots and scripts as needed.
```

<!-- Optional

## Credits

List collaborators, if any, with links to their GitHub profiles.

If we used any third-party assets that require attribution, list the creators with links to their primary web presence in this section.

-->

## How to Contribute

* [Making a Contribition ](CONTRIBUTING.md)
* [Filing an issue](https://github.com/overture-stack/ego/issues)


## Feedback

<!-- 
Do we have a stack overflow, do we want one?
* Ask a question on [Stack Overflow](https://stackoverflow.com/questions/)
-->

* Connect with us on [Slack](http://slack.overture.bio)
* [Upvote](https://github.com/overture-stack/ego/issues?q=is%3Aopen+is%3Aissue+label%3Anew-feature+sort%3Areactions-%2B1-desc) feature requests

<!-- 
Need to consult communications department on social media policy
* Follow [@insertsocials](https://twitter.com/) and let us know what you think!
-->

<!--
Wiki needs updating

See our [wiki](https://github.com/overture-stack/ego/wiki/Feedback) for a description of each of these channels and information on some other available community-driven channels.
-->

<!--
## Known Issues 

Insert any known bugs or issues currently being fixed (can minimize repetative feedback)
-->

## Code of Conduct

<!--This is a standard code of conduct however organizations usually link to one found on there website-->
&emsp; [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)

## License

<!--
Is there OICR copyright?
Copyright (c) OICR. All rights reserved.
-->

Licensed under the [GNU Lesser General Public License v3.0](LICENSE.txt) license.

<!--Optional
## Tests 

Provide examples on how to run them here.
-->
