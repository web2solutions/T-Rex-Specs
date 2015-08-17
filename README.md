# T-Rex Toolkit

> Build rich && high available enterprise web applications

T-Rex is a complete web toolkit and framework.

It lets you to create enterprise web apps in a very short time and with no line of code.

it composed by the following softwares:

 - AgileREST
 - AgileWebsocket
 - Agile Visual Designer
 - $dhx Framework
 - T-Rex webOS

## AgileREST

The AgileRest layer is a high available REST environment built on top of Mojolicious, 
a fantastic and modern Perl framework.

This layer is responsible to provide DB and IO server support for all authenticated clients.

The communication between Client and Server is performed via HTTP in a REST way.
 
This app runs on a pre-forking box, with multiple workers, which may be easily scalated.

It provides asynchronous tasks always as possible.
 
Nginx is in front of the API end points working as load ballancer/proxy.
 
The AgileRest layer provides support for hot deploy of new REST end points.
 
The AgileRest layer provides automatic generated doc for each mapped server resource.

	The generated docs provides all techinal informations about each REST end point.
	
	It provides several working client code samples for all type of operations that 
	are supported by the end point.
 
The AgileRest Layer does not servers static content, which is served via CDN / Nginx.
 
Each server resource is fully protected via HTTP authorizations and tokens

Repository: https://github.com/web2solutions/AgileREST


	RDBMS: PostgreSQL 9.4
	data cache: Redis
	Application language: Perl
	Framework: Mojolicious


## AgileWebsocket

The AgileWebsocket, also built on top of Mojolicious, is a realtime application that is responsible by the messaging system on T-rex.

The back-end is a Redis pub-sub.

This messaging system is used by 3 main tasks:

	- bind and sync between client components X indexedDB X server.
	- propagate application state between connected clients.
	- communication with stand alone server workers.

Repository: https://github.com/web2solutions/AgileWebsocket

	
	MQ: Redis
	Application language: Perl
	Framework: Mojolicious


## Agile Visual Designer

Agile Visual Designer is a very sophisticated RAD/CASE* tool. 



More than that, it is a Database and Web Application designer.

Agile Designer is the responsible tool for creating database tables, 
REST end points, client meta data, generic and complete CRUDL interfaces.

With Agile Visual designer, you are able to build advanced CRUDL applications to be 
automatically integrated on T-Rex webOS with no line of code.

It generates, in seconds, complex applications that you would spend weeks or months writing it.

It provides also, fully and agile support for building custom applications that will 
run and consume resources from T-Rex webOS.

	Front-End: 
	- Language: Javascript
	- Framework: DHTMLX

	Back-End:
	- Application layer: AgileRest
	- data layer: PostgreSQL

* See:

	"https://en.wikipedia.org/wiki/Rapid_application_development" &&

	"https://en.wikipedia.org/wiki/Computer-aided_software_engineering"


## $dhx Framework

 - dhx DataDriver
 - dhx Rest
 - dhx Cruder
 - dhx component proxy
 - dhtmlx modifiers
 - dhx desktop


Repository: https://github.com/web2solutions/dhx

## T-Rex webOS

Repository: It is part of $dhx Framework

### AUTHORS, LICENSE AND COPYRIGHT

 - José Eduardo Perotta de Almeida. eduardo at web2solutions.com.br

  Copyright 2015 

- Commercial licensing only