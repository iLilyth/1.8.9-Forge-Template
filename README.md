# 1.8.9-Forge-Vigilance-Template
A template that's fully functional as of March 31st, 2023 @ 20:00. Uses Shadowjar, Essential, and Vigilance.

All of the Vigilance examples either A. use kotlin B. dont work or C. dont compile. However, this (as of the initial release date) works perfectly.

# Implementation
This was used with no errors on `IntelliJ 2022.3.2`

Repo includes:
```
       java   8
     gradle   6.8.3
     shadow   6.1.0
  minecraft   1.8.9
forgegradle   6f53277
```
# Setup
1. Clone this repository.
2. Import `build.gradle` as a project.
3. Let it configure.
4. run `SetupDecompWorkspace`in Gradle: `Tasks > forgegradle > setupDecompWorkspace`
5. Reload gradle project.
# Build
Run `build` in gradle `Tasks > build > build`
> Note: If the build ever finishes with an error looking like `duplicate entry`, then run clean in Gradle: `Tasks > build > clean`
> Output .jar will be located in build/libs/
# Run
Run `genIntellijRuns` in Gradle: `Tasks > forgegradle > genIntellijRuns`
> This will create the run configurations.
> Note: you will need to change the classpath module to .main
