# Modern Devops: Understanding the terrain

Mitchell Hashimoto, Hashicorp, @mitchellh

## Devops divisions - Application lifecycle

"All applications follow this same general lifecycle."

* Development
    * Readily available
    * Make changes, save changes - Code -> Save -> Reload -> Repeat
    * Consistency "It doesn't work on my machine."
    * Collaboration & Sharing
* Deployment
    * Layers - test, staging, production
    * Start / Configure servers
    * Deploy / Run
        * Compile
        * Get it on the server
        * Start it
        * Make it live or activate it
* Maintenance - Keeping everything running while everything is changing
    * Monitoring
    * Updating
    * Orchestrating - playing well with entire ecosystem

Goal is to make that application lifecycle more efficient.

## Tools

* Reduce human error
* Increase repeatability
* Codification of knowledge
* Faster; more efficient

### Development

Vagrant http://vagrantup.com

* Clone repo
* vagrant up
* go go gadget go

`vagrant share` - return a URL to connect remotely

`vagrant connect` - configure a static IP on the local network

Vagrant prioritizes workflow over technology

### Deployment

Packer http://packer.io

* Start / configure server side of things
* Optimize the slow part of setting up a server by prebuilding them into images
* Devops has been against making machine images (Images are so ten years ago) but...
    * Super fast infrastructure deployment
    * Stability and testability
    * Gets rid of the slow parts

### Maintenance

Serf http://www.serfdom.io/

* Lots of problems and solutions
* Common goal: Change with a resiliency to failure

Serf is a decrentralized, highly available, fault tolerant, and lightweight solution to ...

* Manages membership
* lets you know when something changes - join, leave, fail, change

Example, how to know when a web server is removed from behind a load balancer? (well, health check?) If you're adding? "Serf. It knows things."

* Serf agent on each node
* Handlers
* Actions

How does it work?

* Gossip based member protocol (Example: 4,000 nodes, EC2, 200ms to every node knowing about a new node.)
* Failure detection
    * Not heartbeat
    * Probablistic (Every second, one node chooses another node at random. Can't reach? Ask another node if it could check...)
    * 4,000 nodes on EC2 - 1 second failure detection
* Custom events
    * What to do when something changes
    * Request - Response mechanism

Resilient to failure, near instant orchestration.

Something coming in two weeks.


