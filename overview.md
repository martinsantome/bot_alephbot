# What is this project?
A platform to hold debates. People and bots can talk on this online scenario.

# What you got until date?
- A bunch of nodes on Node-Red to build a webapp ui with two chat forms.
- Some implementation of a cloud.

# What is inside here?
- [Node-red export](node-red-export) file (to be imported on your own node-red server). This is the main website.
- [node-red-ibm-bluemix](node-red-over-ibm-bluemix) Código fuente del tutorial [Bluemix chat in 5 minutes](https://www.ibm.com/developerworks/cloud/library/cl-rtchat-app/index.html).

# Explain the code
## FrontEnd (Plato)
User sees a page with two vertical sections. 

Each section represents a location where a real chat room is located.

On the left, there is a pair of holders to talk.

On the right, a clon.

Each holder contains two bokers.

One for human to speak.

The other for ia to talk.

We can add here as many boxes as consider.

![](overview/000.png)

All this chats are represented on backend as a servers.

### FrontEnd (Bluemix)
![](bluefront.png)

## Backend
On the backend, of course, we are using nodes:
![](overview/dashboard.png)

... to build the user interface... but also nodes to do the transport layer...
![](overview/nodes.png)

Main flow is quite simple for two servers.

![](overview/mapa.png)

On image above you can see two servers, one from Madrid and one for Paris.

Each server consists on two other nodes: "The chat room & a feature-container"

![](overview/server&chat.png)

The server is just a few bunch of nodes.

![](overview/server.png)

The chat is as much simple as that:

![](overview/chat.png)

### Backend bluemix
![](blueback.png)

