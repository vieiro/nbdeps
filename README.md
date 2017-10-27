Maven BOM projects for some third-party dependencies of incubator-netbeans

# Use

    cd netbeans-equinox-bom; mvn install
    cd NBDEPS; mvn dependency:tree

Sample result:

    --- maven-dependency-plugin:2.1:tree (default-cli) @ NBDEPS ---
    org.apache.netbeans:NBDEPS:jar:1.0-SNAPSHOT
    +- org.eclipse.platform:org.eclipse.equinox.preferences:jar:3.7.0:provided
    |  \- org.eclipse.platform:org.eclipse.equinox.common:jar:3.9.0:provided
    +- org.eclipse.platform:org.eclipse.equinox.security:jar:1.2.300:provided
    +- org.eclipse.platform:org.eclipse.equinox.app:jar:1.3.400:provided
    |  \- org.eclipse.platform:org.eclipse.equinox.registry:jar:3.7.0:provided
    +- org.eclipse.platform:org.eclipse.core.contenttype:jar:3.6.0:provided
    +- org.eclipse.platform:org.eclipse.core.jobs:jar:3.9.0:provided
    +- org.eclipse.platform:org.eclipse.core.net:jar:1.3.100:provided
    |  \- org.eclipse.platform:org.eclipse.osgi:jar:3.12.0:provided
    +- org.eclipse.platform:org.eclipse.core.runtime:jar:3.13.0:provided
    \- org.eclipse.core:org.eclipse.core.runtime.compatibility.auth:jar:3.2.200.v20100517:provided
       \- org.eclipse.equinox:org.eclipse.equinox.common:jar:3.6.0.v20100503:provided
          \- org.eclipse.osgi:org.eclipse.osgi:jar:3.6.0.v20100517:provided


# Todo

Create more BOMs for other third party software (mylyn? Apache commons?)

