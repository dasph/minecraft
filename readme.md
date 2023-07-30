# Drew's Minecraft Server

## INSTALLATION

1. Setup a vanilla Minecraft `installation`
2. Install `Fabric` mod loader:
    - download [universal jar installer](https://fabricmc.net/use/installer/) (avoid using `Windows` installer since it requiers a global `JRE` instance)
    - launch the mod loader using `JRE` that was installed by `Minecraft`:
      - nagivate to your `Minecraft` installation
      - go to `runtime/java-runtime-gamma/*os*/java-runtime-gamma/bin/`
      - open a terminal window in the same directory with the `Fabric` mod loader
      - use `java(.exe)` executable from the Minecraft folder to run `fabric-installer-*.jar`: \
      `D:\games\minecraft\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\java.exe -jar fabric-installer-0.11.2.jar`
    - select minecraft version: `1.20.1` and click `install`
3. Install server mods:
    - launch `Minecraft`
    - select `Installations` tab
    - you should see at least two installations: `vanilla` and `fabric`. Hover onto the `fabric` installation and click the `folder` icon
    - you should get navigated into the `fabric` installation folder. Copy the path to the `./mods` folder
    - clone `this` repository and open a terminal window in its root directory
    - download all mods:
      - wget: `wget -i ./extras/.mods -P /PATH/TO/MODS/FOLDER`
      - curl (linux): `xargs -n 1 curl -JOs --output-dir /PATH/TO/MODS/FOLDER < ./extras/.mods`
      - curl (windows): `for /F "delims=" %i in (./extras/.mods) do curl -JOs --output-dir /PATH/TO/MODS/FOLDER %i`
4. Launch `fabric` installation of `Minecraft`
g
