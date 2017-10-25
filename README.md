Maven BOM projects for some third-party dependencies of incubator-netbeans

# Use

    cd netbeans-equinox-bom; mvn install
    cd NBDEPS; mvn dependency:tree

Sample result:

    [INFO] Scanning for projects...
    [INFO]                                                                         
    [INFO] ------------------------------------------------------------------------
    [INFO] Building NBDEPS 1.0-SNAPSHOT
    [INFO] ------------------------------------------------------------------------
    [INFO] 
    [INFO] --- maven-dependency-plugin:2.8:tree (default-cli) @ NBDEPS ---
    [INFO] org.apache.netbeans:NBDEPS:jar:1.0-SNAPSHOT
    [INFO] +- org.eclipse.platform:org.eclipse.equinox.preferences:jar:3.7.0:provided
    [INFO] |  \- org.eclipse.platform:org.eclipse.equinox.common:jar:3.9.0:provided (version selected from constraint [3.2.0,4.0.0))
    [INFO] +- org.eclipse.platform:org.eclipse.equinox.security:jar:1.2.300:provided
    [INFO] \- org.eclipse.platform:org.eclipse.equinox.app:jar:1.3.400:provided
    [INFO]    \- org.eclipse.platform:org.eclipse.equinox.registry:jar:3.7.0:provided (version selected from constraint [3.4.0,4.0.0))
    [INFO] ------------------------------------------------------------------------
    [INFO] BUILD SUCCESS
    [INFO] ------------------------------------------------------------------------
    [INFO] Total time: 1.052 s
    [INFO] Finished at: 2017-10-26T00:31:31+02:00
    [INFO] Final Memory: 12M/239M
    [INFO] ------------------------------------------------------------------------



# Todo

Create more BOMs for other third party software (mylyn? Apache commons?)

