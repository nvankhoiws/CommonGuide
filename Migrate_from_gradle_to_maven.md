This guide you how to convert a gradle project to maven project by follow the below steps:

  ---------------

  **PREREQUISITE**

  In your computer, `jdk`, `maven` and `gradle` must be installed

  -----------
   Please follow step by step:X

  1. Go into directory of gradle project (src root directory)

  2. Open file build.gradle, add this line: `apply plugin: 'maven'`

  3. Open Terminal from the src root directory

  4. Run command: `gradle install`

  5. Go into `build` folder, go deep to folder poms, copy file named `pom-default.xml` to src root directory

  6. You may want rename `pom-default.xml` to `pom.xml` if you like

  7. You can run command `mvn -X clean install package` to check if the conversion is successful

  8. If step 7 is BUILD SUCCESS, you may want to remove all stuff related to gradle such as folder `gradle`, file `settings.gradle`, file `gradle.properties`, file `build.gradle`

  9. This step is not necessary, but i think it may be needed in the case maven conversion is not run or error, and you want use it to debug. You should run command `gradle dependencies > dependencies_tree.txt`. This command will save dependencies tree that gradle does. This step should do before step 2.

  --EOF--


