# Gelf.NET
Gelf.NET is a port from the [gelf4net](https://github.com/jjchiw/gelf4net) project to provide the ability to publish messages to Graylog without any dependencies on other frameworks

[![Build status](https://ci.appveyor.com/api/projects/status/94eeue42c2aggdq6?svg=true)](https://ci.appveyor.com/project/cjbhaines/gelf-net)

## Installation

You can install the latest stable release using the nuget package `Gelf.NET`.

## Usage

	var publisher = new GelfPublisher(remoteHostname: "mygraylogserver.betgenius.com", remoteHostPort: 12201);
	publisher.Publish(new GelfMessage());


# Gelf.NET Standart
Gelf.NET Standart is a port from the [gelf4net](https://github.com/jjchiw/gelf4net) project to provide the ability to publish messages to Graylog without any dependencies on other frameworks

## Installation

Download, Build & Use

## Usage

	var publisher = new GelfPublisher(remoteHostname: "mygraylogserver.betgenius.com", remoteHostPort: 12201);
	publisher.Publish(new GelfMessage());

# Remarks

Due to the C# UdpClient not guaranteeing thread safety, you should also assume that the GelfPublisher is not thread safe.

