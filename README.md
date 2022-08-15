# Mock Repository Manager: Project

> :warning: This repository is a fork of the Mock Repository Manager that is maintained by [Corgibytes](https://corgibytes.com). It includes a [pull request](https://github.com/mojohaus/mrm/pull/117) that hasn't yet been merged into the upstream project. If that pull request gets merged, then this fork will likely be removed.

Mock Repository Manager for Maven. The Mock Repository Manager provides a mock Maven
repository manager.
 
[![Apache License, Version 2.0, January 2004](https://img.shields.io/github/license/corgibytes/mrm.svg?label=License)](http://www.apache.org/licenses/)
[![Maven Central](https://img.shields.io/maven-central/v/com.corgibytes/mrm.svg?label=Maven%20Central)](https://search.maven.org/artifact/org.codehaus.mojo/mrm)
[![GitHub CI](https://github.com/corgibytes/mrm/actions/workflows/maven.yml/badge.svg)](https://github.com/mojohaus/mrm/actions/workflows/maven.yml)

## Releasing

* Make sure `gpg-agent` is running.
* Execute `mvn -B release:prepare release:perform`

For publishing the site do the following:

```
cd target/checkout
mvn verify site site:stage scm-publish:publish-scm
```
