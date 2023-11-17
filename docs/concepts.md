---
sidebar_position: 2
title: Concepts
---

## Clusters 

Clusters are the higher level component managed by Launchbox. Each project (guest) gets allocated to an available cluster (host).
Currently, these are pre-existing clusters that our operator is deployed to. Deploying new managed clusters automatically is in our roadmap

### Projects 

Projects represent our unit of work. Each project maps 1:1 with an ephemeral cluster. These can then be configured using:

- Standard tooling, ala `kubectl` and `helm` 
- Installing Addons and Packages through LaunchboxHQ
- Importing project requirements from a [Catalog](#catalogs)

### Catalogs 

These represent the full dependency needs for a given project / service. They are stored as a `launchbox.y[a]ml` file somewhere
in your service. It can then be used to create a project either through the UI, or from our CLI tool 

### Addons / Addon Subscriptions

Addons represent an installable package to be used as a dependency for your service. Things such as Redis, PostgreSQL, 
MinIO, etc. 

When an addon is installed at the project level, this is surfaced as an `Addon Subscription`

### Services

Services usually map to a given VCS repository. They are defined with a deployment spec, and when attached to your project,
are automatically deployed to your cluster. If configured, they are also synced to various sources to update when your remote does

## Organizations

Organizations represent a grouping of teams / users inside of LaunchboxHQ. They can deploy their own addon configurations, 
manage and deploy to private clusters, and take control of much more configuration inside of HQ

