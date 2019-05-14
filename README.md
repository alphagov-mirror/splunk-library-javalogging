# Splunk Logging for Java

This is a fork of [Splunk's java logging library](https://github.com/splunk/splunk-library-javalogging). It was originally
forked so we could enhance it to allow the configuration of the Apache http client used by the library, specifically the 
http proxy settings. The aim is to get this change merged upstream.

#### Version 1.1.0

Splunk logging for Java enables you to log events to HTTP Event Collector or to a TCP input on a Splunk Enterprise instance within your Java applications. You can use three major Java logging frameworks: [Logback](http://logback.qos.ch), [Log4j 2](http://logging.apache.org/log4j/2.x/), and [java.util.logging](https://docs.oracle.com/javase/7/docs/api/java/util/logging/package-summary.html). Splunk logging for Java is also enabled for [Simple Logging Facade for Java (SLF4J)](http://www.slf4j.org).

Splunk logging for Java provides:

* Appender classes that package events into the proper format for the input type you're using (HTTP Event Collector or TCP).

* Handler classes that export the logging events.

* An optional error handler to catch failures for HTTP Event Collector events.

* Example configuration files for all three frameworks that show how to configure the frameworks to write to HTTP Event Collector or TCP ports.

* Support for batching events (sent to HTTP Event Collector only).</li>

### Packaging and publishing

The library is [built, packaged and published by Concourse](https://deployer.tools.signin.service.gov.uk/teams/main/pipelines/build-libraries/jobs/build-splunk-library-javalogging). It's published to both of alphagov's 
bintray and artifactory. When making changes you need to manually bump the version in the pom.xml. Creds for bintray and 
artifactory are pulled from the Concourse environement.

### Requirements

Here's what you need to get going with the Splunk SDK for Java.

#### Splunk

If you haven't already installed Splunk, download it
[here](http://www.splunk.com/download). For more about installing and running
Splunk and system requirements, see
[Installing & Running Splunk](http://dev.splunk.com/view/SP-CAAADRV).

#### Java 

You'll need Java version 7 or higher, from [OpenJDK](https://openjdk.java.net) or [Oracle](https://www.oracle.com/technetwork/java).

## Documentation and resources

* For more information about installing and using Splunk logging for Java, see
  [Overview of Splunk logging for Java](http://dev.splunk.com/goto/sdk-slj).

* For reference documentation, see the
  [Splunk logging for Java API reference](https://docs.splunk.com/DocumentationStatic/JavaLogging/1.6.2/index.html).

* For all things developer with Splunk, see the
  [Splunk Developer Portal](http://dev.splunk.com).

* For more about about Splunk in general, see
  [Splunk>Docs](http://docs.splunk.com/Documentation/Splunk).

## License

Splunk logging for Java is licensed under the Apache License 2.0.

See the [LICENSE file](/license.md) for details.

## Contributions

[Get the Splunk Java Logging Framework from GitHub](https://github.com/splunk/splunk-library-javalogging)
and clone the resources to your computer. For example, use the following
command:

    git clone https://github.com/splunk/splunk-library-javalogging.git

## Support

The Splunk logging for Java is community-supported.

1. You can find help through our community on [Splunk Answers](http://answers.splunk.com/) (use the "logging-library-java" tag to identify your questions).
2. File issues on [GitHub](https://github.com/splunk/splunk-library-javalogging/issues).

## Contact us

You can reach the Dev Platform team at [devinfo@splunk.com](mailto:devinfo@splunk.com).
