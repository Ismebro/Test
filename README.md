# Mcberdasi Addon

One combined Meteor Client addon project. Future features should be integrated into this project, not published as separate addon JARs.

## Current module: Fake Lag

Settings currently included in source:
- Mode: Constant, Random, Pulse
- Constant delay (50–2000 ms)
- Random delay minimum and maximum
- Pulse hold and release durations
- Only player movement packets are intercepted; chat and interactions are left alone
- Maximum queued packets
- Flush queued packets on disable

This is intended for private-server or controlled network testing. It does not bypass anti-cheat; servers can correct movement or disconnect clients.

## Target
- Minecraft Java 1.21.11
- Java 21
- Fabric Loader 0.18.4
- Meteor Client 1.21.11 snapshot

## Build
The GitHub Actions workflow builds the project with Java 21 and Gradle 8.14.3. Push this project to a GitHub repository and run the workflow from the Actions tab.

**Build status:** source files have been updated, but this environment has not compiled the project or tested the module in Minecraft. Meteor's published 1.21.11 snapshot and API compatibility must be confirmed by the remote build.
