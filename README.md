## Purpose

Control all your servers over github.
This is a template repo.

## Secrets

| Name                       | Value                                                                                 |
|----------------------------|---------------------------------------------------------------------------------------|
| PAT_READ_PACKAGES          | A PAT that allows this package to access your github container registry               |
| MAIN_SERVER_SSH_PASS       | Your servers user password (ssh)                                                      |
| MAIN_SERVER_SSH_USER       | Your servers user name (ssh)                                                          |
| IP_ADDRESS                 | Your servers ip address                                                               |
| ENVIRONMENT_VARIABLE_ONE   | If you need environment variables for your apps, this is how to pass the vars to them |

## Clear orphaned containers
Your server might get some orphaned containers over time. You can clear them by manually connecting to your server via ssh and running the following command `docker rm -f $(docker ps -a -q)`
