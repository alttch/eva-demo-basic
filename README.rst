EVA ICS demo: Basic
*******************

EVA ICS (https://www.eva-ics.com/) basic demo configuration.

Layout
======

This demo deploys single EVA ICS node with UC, LM PLC and SFA installed.

The node configuration is empty.

Network and containers
======================

* **eva_basic_1** EVA ICS node, *10.27.5.10:*

Deployment
==========

Requirements: `Docker <https://www.docker.com/>`_, `docker-compose
<https://docs.docker.com/compose/>`_.

* Execute *docker-compose up* to deploy containers

Management
==========

http://10.27.5.10:8828 - SFA API/primary operator interface (empty, framework
files only).

From the command line: *docker exec -it eva_basic_1 eva-shell*

The default master key is: *demo123*

Components:

* http://10.27.5.10:8812 - UC API/EI
* http://10.27.5.10:8817 - LM PLC API/EI

Volumes
=======

All permanent volumes are created and mounted from ./data directory.
