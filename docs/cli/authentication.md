---
sidebar_position: 2
title: Authentication
---

## Personal Access Token 

Most CLI uses cases will authenticated with a personal Access Token. You can generate one at https://launchboxhq.io/access_tokens

```shell 
export LAUNCHBOX_ACCESS_TOKEN="<my-personal-access-token>"
launchboxctl projects list
```

## Client Credentials 

This authentication mechanism is mostly reserved for cluster communication with HQ.

```shell 
export LAUNCHBOX_CLIENT_ID="<my-client-id>"
export LAUNCHBOX_CLIENT_SECRET="<my-client-secret>"
launchboxctl projects get --project-id xxx
```
