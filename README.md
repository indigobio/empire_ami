# empire_ami
Home of the AMI building tools for the Official Empire AMI

In order to run the AMI, you'll need to create the file /etc/empire/seed via user data on boot with the following variables:

## For controllers

```
EMPIRE_HOSTGROUP=controller
EMPIRE_DATABASE_USER
EMPIRE_DATABASE_PASSWORD
EMPIRE_DATABASE_HOST
EMPIRE_GITHUB_CLIENT_ID
EMPIRE_GITHUB_CLIENT_SECRET
EMPIRE_GITHUB_ORGANIZATION
EMPIRE_TOKEN_SECRET
EMPIRE_ELB_SG_PRIVATE
EMPIRE_ELB_SG_PUBLIC
EMPIRE_EC2_SUBNETS_PRIVATE
EMPIRE_EC2_SUBNETS_PUBLIC
EMPIRE_ECS_SERVICE_ROLE
EMPIRE_ROUTE53_INTERNAL_ZONE_ID
ECS_CLUSTER
DOCKER_USER
DOCKER_PASS
DOCKER_EMAIL
DOCKER_REGISTRY
```

and optionally

```
ENABLE_STREAMING_LOGS
```

## For minions

```
EMPIRE_HOSTGROUP=minion
ECS_CLUSTER
DOCKER_USER
DOCKER_PASS
DOCKER_EMAIL
DOCKER_REGISTRY
```

and optionally

```
ENABLE_STREAMING_LOGS
```
