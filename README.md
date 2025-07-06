This is a JetBrains IDE theme plugin inspired by [Solarized](https://ethanschoonover.com/solarized/) and [Ayu](https://github.com/dempfi/ayu)

You can install the plugin directly by selecting Install Plugin from Disk and choosing the Solar-Ayu.jar

The font shown in the screenshots is "SF Mono" by Apple Inc. Please note that it is subject to strict copyright restrictions. Alternatively, you may consider using JetBrains Mono.

If you want to motify colors, there two key files in the project: 

theme/SolarAyu.theme.json — defines the overall IDE colors
colors/SolarAyu.xml — defines the editor area colors

(.icls files, which you may find in some projects, are XML-based and essentially equivalent to .xml files. You can rename them directly.)

If you want to add new editor colors, you can create another .xml file and add following lines in the META-INF/plugin.xml(replace the file name accordingly)
```
<extensions defaultExtensionNs="com.intellij">
    <themeProvider id="Solar-Ayu" path="/theme/SolarAyu.theme.json"/>
</extensions>
```
There are differences between the keywords used in the IDE settings and those in the .xml files, and the official documentation and examples do not offer adequate support. The comments I write in .xml file maybe can help you.

Have fun!

