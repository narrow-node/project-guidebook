# Guidebook for Uniform Project Systems

###### :warning: Following this guidebook will be mandated for all Narrow Node projects.

In order to establish consistency across project structures, this document will outline what needs to be done for each new project. In the following walkthrough, we will create a sample project structure that aims to put a man on Mars. The project name for this will be `Mars Landing` and contains the following components:
- Build a mainframe calculator
- Build a fuel capacitor
- Build a manufacturing machine

Given a project name and basic goals, structured conventions will be used to organize the project.

## Table of Contents
1. [Create a Narrow Node Project](#1-create-a-narrow-node-project)
2. [Creating Project Repositories](#2-creating-project-repositories)
   1. [Create a wiki repo](#create-a-wiki-repo)
   2. [Create component repos](#create-component-repos)
3. [Planning Project Direction](#3-planning-project-direction)
   1. [Create Yellow and White Paper](#create-yellow-and-white-paper)
   2. [Creating Diagrams](#creating-diagrams)
4. [Managing Development](#4-managing-development)
   1. [Staff](#staff)
- [Current Projects](#current-projects)

## 1. Create a Narrow Node Project
Start by going to the [`narrow-node` projects page](https://github.com/orgs/narrow-node/projects) and click `New Project`. The sample project name would be `Mars Landing` for the project board name.

This will be where to-do lists can be managed for the project later on.

## 2. Creating Project Repositories
All repositories will have an explicit naming structure and will be within the [`narrow-node` organization page](https://github.com/narrow-node). Before creating any repository, make sure it is done from that page.

### Create a wiki repo
This will be the main repository for the entire project. It will serve as a wiki for project-wide documentation. Title this repository as `mars-landing`, the name of the repository being in lowercase with hyphens replacing spaces. Leave this repository blank for now.

### Create component repos
For each component of the project, a new repository will be created. They should each be named as the first word of the project name, and then a second word summarizing that component's function. For the `Mars Landing` project, the microservice repos to create will be:
- `mars-mainframe`
- `mars-capacitor`
- `mars-machine`

After creating a repository for each component, also leave them blank for now.

## 3. Planning Project Direction
### Create Yellow and White Paper
The project wiki repository `mars-landing` will start with two pages:
- `Yellow Paper` Research paper outlining underlying tech and repositories
- `White Paper` Content creation paper showcasing feature and version planning

In the wiki `mars-landing` repository, click `Wiki`, then `New Page` for each paper.

Both of these papers must be written in the wiki repo before any code or other documentation is written. They will provide planning for the entire lifetime of the project, and are great to be used as a reference throughout development. It is critically important that they are thorough and nothing is overlooked. See [Current Projects](#current-projects) for examples of Yellow and White Papers.

### Creating diagrams
Use [draw.io](https://draw.io) to make all diagrams so that they look uniform. Use `Courier New` as the only font. Export them as an image with the `Shadow` option enabled, and upload them to the wiki repo `mars-landing` under a folder titled `diagrams` so that all documentation can reference them.


## 4. Managing Development

### Staff
All Narrow Node projects will use the following staff groups:
- [Owners](https://github.com/orgs/narrow-node/teams/owners)
- [Developers](https://github.com/orgs/narrow-node/teams/developers)
  - [Designers](https://github.com/orgs/narrow-node/teams/designers)
- [Moderators](https://github.com/orgs/narrow-node/teams/moderators)
- [QA](https://github.com/orgs/narrow-node/teams/qa)

`Owners` are developers that must audit more sensitive code before it is accepted.

`Developers` specialize on a component of the game writing code.

`Designers` are primarily responsible for wiki and content creation. but won't be writing any code.

`Moderators` are community managers that don't have any elevated permissions in terms of content creation.

`QA` are alpha and beta-testers for fragile content that isn't yet released.

---
## Current Projects
- [`paperweight`](https://github.com/narrow-node/paperweight/wiki/)
