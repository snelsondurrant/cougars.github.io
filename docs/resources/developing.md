---
layout: default
title: Developing
nav_order: 2
parent: Resources
---

# Developing

---

## Software Development
\
To start developing for the Coug-UV, simply clone [https://github.com/snelsondurrant/CougarsRPi.git](https://github.com/snelsondurrant/CougarsRPi.git) or [https://github.com/snelsondurrant/CougarsTeensy.git](https://github.com/snelsondurrant/CougarsTeensy.git) (depending on what you're working on), make a new branch, and start coding and pushing some changes.

Helpful information on code structure is included in the "README.md" files for both GitHub repos, in addition to header comments in other important files.

{: .note }
> The Docker image running on the vehicles should automatically re-load the latest git commit from "main" on startup (as long as it has an internet connection). Before a field test, however, the Docker image should be re-pushed to "snelsondurrant/cougars:latest" with the current software updates and loaded locally onto the Coug-UV by using the "docker.sh" script.
>
> There's probably an automated way to do that, but I haven't found a great solution yet.