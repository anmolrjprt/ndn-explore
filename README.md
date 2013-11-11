NDN Explore

This utility issues recursive queries in the style of the 'ndnls' command line utility to explore the naemspace.

Dependencies:

1. NDN-JS (Link: https://github.com/named-data/ndn-js)
2. JSTree Pre1.0 (Link: https://github.com/vakata/jstree/tree/v.pre1.0)

Connectivity:

For Javascript API, a websockets proxy that can communicate the target ndnd is currently required. It currently 
listens on port 9696 and passes messages to ndn daemon to which it is routed. This application connects to websocket
proxy B.ws.ndn.ucla.edu(over port 9696) which is routed to borges.metwi.ucla.edu

Description:

The NDN Exlpore is a browser based tool with ndnls like functionality for NDNx. This tool is written using NDNJS 
library for exploring the namespace in ndnx nodes. It enables the user to browse through the namespace 
in a more intuitive and interactive fashion. 

Usage : 

The tool on clicking a particular node adds the first level names(suffix) under that prefix.

On clicking on an already expanded node the child nodes get deleted. 

Whenever a user clicks on a child node with no child(suffix), the content is displayed in the content box below 
tree structure. In other words, as soon as the user traverses the complete name of a data object and clicks on 
the last node(suffix), the content of that data object is displayed in the box below box displaying tree structure.

The application also provides the user to choose maximum number of child nodes to list whenever the node is clicked.

Note: 

The browser must be able to connect to remote port 9696, which may not be enabled on some firewalls.




