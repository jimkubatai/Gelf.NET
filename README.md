# Gelf.NET Standart
Gelf.NET Standart is a port from the [Gelf.NET](https://github.com/geniussportsgroup/Gelf.NET) project to provide the ability to publish messages to Graylog without any dependencies on other frameworks

## Installation

Download, Build & Use

## Usage

	var publisher = new GelfPublisher(remoteHostname: "mygraylogserver.betgenius.com", remoteHostPort: 12201);
	publisher.Publish(new GelfMessage());

## Remarks

Due to the C# UdpClient not guaranteeing thread safety, you should also assume that the GelfPublisher is not thread safe.

