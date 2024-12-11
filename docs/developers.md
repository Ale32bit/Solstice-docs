# Developers

Would you like to interface with Solstice?

Add the Maven repository:

```groovy
maven {
    name "alexdevs"
    url "https://maven.alexdevs.me/releases"
}
```

...and add the dependency:

```groovy
// Solstice Essentials
modImplementation "me.alexdevs:solstice:VERSION"
```

Replace `VERSION` with the preferred version. eg. `1.0.0+1.20.1` (without `v`).