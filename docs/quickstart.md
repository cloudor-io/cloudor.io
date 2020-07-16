# Quick Start

## Prerequisite

You need a docker image

## Hello World

- Three easy steps:
    1. Download the command line tool `cloudor` from github:
        * Mac OS X
            ```bash
            brew ...
            ```
        * Linux x64 64-bit
            ```bash
            ```
        * Windows 64-bit
            ```
            ```
    2. Register. Run the following command and follow the prompt to set up your user account:
        ```bash
        $ cloudor user login
        ```

    3. Run a `hello world` job
        ```bash
        cloudor run cloudor/hello-world:latest --vendor aws --region us-east-1 --instance-type xlarge TODO
        ```

## Console

The web console service is avaialble at https://cloudor.dev. It can be used to:

* View basic user profile and credit
* View recent jobs
* View recent credit transactions
* Make payment
