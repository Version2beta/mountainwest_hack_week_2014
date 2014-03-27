# Bridging Devops with Pantry

Jason Roelofs, Collective Idea, @jasonroelofs

What is Pantry?

* Pipeline / Automation framework
* Convention over configuration
* Use tools of your choice
* NOT a configuration tool. It uses configuration tools.

Chef server - organizations don't share cookbooks.

Devops is a collection of islands, little connection between tools and ecosystems.

New Stack Questions

* Where do I store data
* How provision
* How configure?
* How share configs?
* How to secure?

Enter Pantry

* Gem
* Pantry::Client
    * Run commands
    * All, some or one
    * Can run chef and other plugins
* Pantry::Plugins

Security
* The default is none
* Not openssl
* Opt-in to CurveZMQ instead - using CurveCP, elliptical curve cryptography, http://curvezmq.org


