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
   3. [Versioning](#versioning)
   4. [Creating Update Packs](#creating-update-packs)
   5. [To-Do Lists](#to-do-lists)
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

### Creating Diagrams
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

### Versioning
Version numbers will use [npm's semantic versioning](https://docs.npmjs.com/getting-started/semantic-versioning) conventions. They are structured like so:

`vX.Y.Z`

- `X` Major, potentially breaking updates that shift to a new `Update Phase` (more in a moment)
- `Y` Minor, non-breaking updates containing `Update Packs` that do not introduce a new `Update Phase`
- `Z` Bug fix(es)

Each number starts at `0`, and increments indefinitely until its parent increments. So, if `Mars Landing` was `v2.7.29`, then it is version `2`, with `8` update packs and `30` bug fixes. When there is a new update pack, it becomes `v2.8.0`, and when there is a new 
update _phase_ it becomes `v3.0.0`.

Versions are **not** repository specific. Keep version numbers uniform across all repositories. If updates have occured on `mars-manufacturing` and `mars-capacitor` but not on `mars-mainframe`, the `mars-mainframe` version should be updated anyway. This may seem odd, but it will becomre more apparent.

To modify the versions on each repository, use the `Releases` tab.

`Update Phases` are names for major version changes. For `Mars Landing` there may be the following phase names and versions:

0. Liftoff
1. Breakthrough
2. Orbit
3. Landing

So in the `Releases` tab for each repository, when `v2.0.0` is released, the title name for that tag becomes `Orbit`. This is why each repository needs a consistent version. Update phases mark significant milestones throughout the project and have unique visionary strategies. Some phases may be considered expermential, some stable, and some permanent.

### Creating Update Packs
For larger, more comprehensive to-do lists such as biweekly update packs, go to `Projects` for the repository being updated. If `mars-mainframe` needed update pack #2 to be documented, a new project could be created _within that repository_. To be clear, this is not the same as the `Projects` tab under the Narrow Node organization page. The `Project board name` for the update pack would be `Liftoff v0.2.0 - Ship measurement calculator` and the description would contain a markdown checklist of everything that needs to be added for the update pack.

### To-Do Lists
Automate to-do lists for bug-fixes and wiki pages by opening an issue inside the repository and creating a markdown checklist inside the new issue post. On the right, assign the issue to the project. This will automatically add it to the `Mars Landing` To-Do section in the Narrow Node Projects page.

### Communicate with team members!!!
Say what you are feeling, even if it is unpopular. Never just go along with an update if you feel it is bad for the project.

---

## Current Projects
- [`paperweight`](https://github.com/narrow-node/paperweight/wiki/)
