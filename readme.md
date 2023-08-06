# Drew's Minecraft Server

## INSTALLATION

1. Setup a vanilla Minecraft installation
2. Install `Forge` mod loader:
    - download the [jar installer](https://maven.minecraftforge.net/net/minecraftforge/forge/1.19.2-43.2.21/forge-1.19.2-43.2.21-installer.jar)
    - launch the mod loader using `JRE` that was installed by Minecraft:
      - navigate to your `Minecraft` installation
      - go to `./runtime/java-runtime-gamma/*os*/java-runtime-gamma/bin/`
      - open a terminal window in the same directory with the `Forge` mod loader
      - use `java(.exe)` executable from the Minecraft folder to run `forge-1.19.2-43.2.21-installer.jar`: \
      `D:\games\minecraft\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\java.exe -jar forge-1.19.2-43.2.21-installer.jar`
    - click **OK**
3. Install server mods:
    - launch `Minecraft`
    - select **Installations** tab
    - you should see at least two installations: **vanilla** and **forge**. Hover onto the **forge** installation and click the **folder** icon
    - you should get navigated into the **forge** installation folder. Copy the path to the `./mods` folder
    - clone this repository and open a terminal window in its root directory
    - download all mods:
      - wget:
        ```
        wget -i ./extras/.mods -P /PATH/TO/MODS/FOLDER
        ```
      - curl (linux):
        ```
        xargs -n 1 curl -JOs --output-dir /PATH/TO/MODS/FOLDER < ./extras/.mods
        ```
      - curl (windows):
        ```
        for /F "delims=" %i in (./extras/.mods) do curl -JOs --output-dir /PATH/TO/MODS/FOLDER %i
        ```
4. Launch `forge` installation of `Minecraft`
