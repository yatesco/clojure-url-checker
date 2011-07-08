# What is all this?
Primarily this is a learning tool to teach me how to use Clojure to build Enterprise Apps.  This clearly isn't an Enterprise App :), but it is a play-ground for me to experiement.  As such, the requirements are driven by my need for an DevOps tool but also as a play-ground for "how do I do this in Clojure".

The hardest thing I have found in thinking about how to use Clojure is what the shape of the solution should look like.  I have spent over a decade training my mind to see (Java) Objects everywhere, both in the design and implementation.  This needs some re-learning, and this is (one of) the tool(s) to do that.

# Real tool
As well as being a learning tool, this tool will also serve a useful Operations Management goal - ensuring that our internally hosted web sites are available to the outside world.  We currently use [pingdom](http://pingdom.com) but this has a few warts.  In the short term, this will be over-engineered.  In the long term, this might just turn out to be quite a useful little tool.
The tool itself will be a web app which can be configured with a list of URLs to check.  A web page will display the statuses of those URLs.

This tool will be heavily inspired (at least at the beginning) by http://pragprog.com/magazines/2011-07/create-unix-services-with-clojure

## Future
Initially this tool will be an over-engineered tool with a single web page.  In the future, it _may_ grow to be quite rich:

- Check network resources other than URLs (maybe even branching into nagios or zabbix territory here, which is fine)
- External DSL (probably using ANTLR) for defining resources to check
- Extensible notification mechanism (probably event-based so listeners respond to "resourceDown" events etc.)
- Push based web app (using COMET?  No idea) rather than Ajax based pull model

# Goals
- Solve a problem we currently have (monitoring our services)
- Sandbox for learning Clojure the language and eco-system (libraries, build-tools)
- See what happens when an old OO dude tries to wear functional glasses 
