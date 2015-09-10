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

The back-end is a Redis pub-sub. (RabbitMQ coming soon)

This messaging system is used by 3 main tasks:

	- bind and sync between client components X indexedDB X server.
	- propagate application state between connected clients.
	- communication with stand alone server workers.

Repository: https://github.com/web2solutions/AgileWebsocket

	
	MQ: Redis (RabbitMQ coming soon)
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

	https://www.youtube.com/watch?v=mHSa_5qI1Ps

	"https://en.wikipedia.org/wiki/Rapid_application_development" &&

	"https://en.wikipedia.org/wiki/Computer-aided_software_engineering"


## $dhx Framework

 - dhx DataDriver
 - dhx Rest
 - dhx Cruder
 - dhx component proxy
 - dhtmlx modifiers
 - dhx desktop (T-Rex webOS)


Repository: https://github.com/web2solutions/dhx

## T-Rex webOS

T-Rex webOS, is a Javascript application which offers a full featured enterprise environment.

It include features like:

 - Server and client database with a very sophisticated data types, data validation and data sync system.
 - Share database and tables through multiple applications
 	Developers will not care about data models, focusing only on controller and view for every new created application
 - Syncing and binding components
 - client state persistance through websocket and RabbitMQ
 - shared REST communication with server
 - shared websocket communication with server
 - User management and permissions
 - Personal user settings
 - Localization - US and BR. It's very easy to create your own localization.
 - Latinization of forms
 - Built in PDF viewer
 - Built in PDF export for grids
 - Built in CSV export for grids
 - RAD designer
 - File Explorer application
 - Webmail
 - Authentication over HTTP
 - Easy installation of plugins (Javascript modules)
 - Easy installation of custom applications (Javascript modules)

The webOS offers 4 main type of applications

 - T-Rex built in applications
 	- Complete search over all data and applications though a ominibox
 	- User preferences application
 	- File Explorer

 - Cruders

 	Cruders are generated CRUDs designed at Agile Visual Designer. 
 	It provides a full CRUD interface for every maped table.

 	The generated cruds provide rich form validations and masks, 
 	
 	rich validation and masks for grid cells.
 	
 	sophisticated uploader system with validation and limit of files.

 	There is also available, a 'preview file system' built in on every section of cruds where you are viewing records.

 - Plugins

 	Plugins are Javascript applications which may be created by any person using Javascript and module pattern.
 	
 	Plugins are started when T-Rex starts.

 	Every plugin has it own button on T-Rex's Top Bar which will be responsible by rendering the plugin's view.
 	
 	It may have or not a button on T-Rex's Left Side Bar


 - Custom application

 	Custom applications are Javascript applications which may be created by any person using Javascript and module pattern.
 	
 	Applications are started when you clicks on it icon.
 	
 	Every application has it own button on T-Rex's Left Side Bar which will be responsible by starting the application calling it start() method from application's controller.




 #### Note:


 	T-Rex offers directly access to the data model for every registered plugins. 

 	It means, except when the developer need to created a new database table, he will not need worry about the model of the application,
 	keep focusing on the controller and view layer only. 

 	It has available also,  all meta data for DHTMLX forms for every table on the shared database. It means developer will may take advantage of T-Rex even for designing him application's forms

Repository: T-Rex is built on top of $dhx framework, under the namespace $dhx.ui.desktop


https://www.youtube.com/watch?v=_m1HhH4l5HA

### AUTHORS, LICENSE AND COPYRIGHT

 - José Eduardo Perotta de Almeida. eduardo at web2solutions.com.br

  Copyright 2015 

- Commercial licensing only