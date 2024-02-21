# mps-javafx

Adding back the removed JavaFX libraries to JetBrains MPS (>= 2020.3)

## Usage

1. Download the [latest zip file](https://github.com/DSLFoundry/mps-javafx/packages/1244402)
2. Unpack the zip in the plugins folder of your MPS distro
3. Add JavaFX as a dependency to your language
4. Import the JavaFX stubs in your models where you want to use JavaFX

## References

- [How to Add JARs to a Jetbrains MPS Project](https://tomassetti.me/how-to-add-jars-and-resources-in-a-jetbrains-mps-project/)
- [Where do I put my jars](https://specificlanguages.com/posts/2022-03/04-where-do-i-put-my-jars/)

## Migrating & Building
1. Open in new MPS
2. Execute migrations
3. Rebuild build solution in MPS
4. Adapt build.gradle dependencies (matching with new MPS)
5. Adapt version number for the javafx plugin in gradle.properties
6. Run ./gradlew to check that it is fine
7. Merge to main and this will release the plugin
