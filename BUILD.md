# Build Instructions

## Create new Splunk Application Bundle

* Update version number in `gradle.properties`

```version=1.0.0```

* Run gradle:

```./gradle createDist

distName: vectra_cognito-1.0.0.spl
destinationDir: <repositorypath>/vectra_cognito/build/distributions
:createDist

BUILD SUCCESSFUL

Total time: 0.993 secs```

* A new `vectra_cognito-<version>.spl` package will be created in the build/distributions directory

## Prepare app certification

* Install AppInspect Toolkit [http://dev.splunk.com/view/appinspect/SP-CAAAE9U]

* Run inspectDist

```./gradle inspectDist```
