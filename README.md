# fluffy-nemesis
`fluffy-nemesis` is a work-in-progress collection of scripts and software to make setting up and administrating I2P nodes easier. 

###Current Features:
* Unfortunately, right now, this repo is pretty empty.

###Todo
1. Headless (SSH-only, menu-based) initialization of Tor and I2P nodes
1. Agent for managing servers (`fluffyd`)
1. Control panel for administrating multiple nodes 
1. Management via the cipherspace connection (no direct connections after initial setup)

##`fluffyd`
`fluffyd` will be an agent that can be run on a cipherspace node, which will make itself available only over the cipherspace connection. This means that once the node has been set up, management can be done entirely over the encrypted and anonymized connections provided by the Tor and I2P networks.

###Wishlist
1. Stage changes on one `fluffyd` server to be applied to another `fluffyd` server that is down at the time the changes are applied ("mesh" capabilities)
1. Switch management messages across networks randomly to provide further anonymity
1. Send fake (NOP) management messages at random intervals, both from `fluffyd` instances and from the control panel to help prevent timing-correlation attacks, or at least make themfar harder.