# eclipse-rcp-with-async-logging

Example project showing how to set up asynchronous logging with Log4j 2 in an Eclipse 3.x application

This is the source code for a tutorial available at http://blog.sdruskat.net/log4j2-in-eclipse-rcp-with-async-loggers/.

## Build and run

Build in the following order.

#### 1. Build Maven projects.
```
 sun-misc-system-bundle-fragment/pom.xml: mvn clean install
 p2-project/pom.xml:                      mvn p2:site
```

#### 2. Add the following to your target platform in Eclipse.

From http://download.eclipse.org/releases/mars:
- Eclipse Platform
- Eclipse RCP

From the newly built p2 repository (p2-project/target/repository):
- Both plugins

#### 3. Load target platform.

#### 4. Run net.sdruskat.blog.rcp.asynclog4j2/net.sdruskat.blog.rcp.asynclog4j2.product. 

This will create a run configuration. Depending on your settings you may have to add required plug-ins (**Run > Run Configurations...** > Tab "Plug-Ins" > Button "Add required plug-ins").
