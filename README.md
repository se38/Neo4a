# Neo4a
The [Neo4j](http://neo4j.com) ABAP Connector

See [Blog post on SAP Community Network](http://scn.sap.com/community/developer-center/cross-technology/blog/2015/01/23/neo4a-the-neo4j-abap-connector)
 
* Nugget: ZNEO4A-x.x.nugg
 
## Required Packages
* Netweaver ABAP Stack 7.40 SP8 or higher
* Neo4j 2.1.6 or higher (lower versions may work but not tested)
* [zJSON The ABAP JSON Document class](https://github.com/se38/zJSON) Version 2.28 or higher
 
## Neo4j Server configuration
If you have installed Neo4j on a separate host (other than the SAP system): to access the database from outside (browser + SAP), you have to change one line of the server configuration file ./conf/neo4j-server.properties:
Enter or uncomment the following line:
```
org.neo4j.server.webserver.address=0.0.0.0
```
You can enter the IP address of your SAP server or leave 0.0.0.0, which means that Neo4j is accessible from every other IP address (not recommended in production!)

## Installation Neo4a
import Nugget with [SAPlink](http://www.saplink.org)

## Usage
see wiki ( https://github.com/se38/Neo4a/wiki )

## License
This software is published under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)
