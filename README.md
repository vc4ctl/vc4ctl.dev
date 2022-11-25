---
description: Command-line tool for Crestron VC-4
---

# VC4CTL

Vc4ctl is a command-line tool for interacting with the REST API of [Crestron VC-4](https://www.crestron.com/Products/Control-Hardware-Software/Software/Licensing/VC-4-ROOM) control servers in a similar manner to tools like kubectl for Kubernetes.

Multiple servers can be configured for control, but only one server at a time may be controlled using vc4ctl.&#x20;

All basic CRUD (create, read, update, & delete) functions are supported for individual programs and rooms. In addition, the tool is able to monitor the status of running rooms, including device status.

The tool also allows for batch uploading of programs, including the various files allowed by Crestron, and batch creation of rooms. Vc4ctl ensures that the programs and all associated files are uploaded prior to creation of rooms using the programs.&#x20;

