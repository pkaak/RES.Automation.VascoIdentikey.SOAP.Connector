# RES.Automation.VascoIdentikey.SOAP.Connector
Vasco Identikey Server SOAP connector for RES Automation
Version 1.0.0 - 19 april 2017
By Patrick Kaak (p.kaak@res.com)


Requirements:
Vasco Identikey Enterprise with SOAP installed

For the connector to work you need an:
- SOAP URL (normally: https://ServerIP:8888)
- account with admin rights on the Vasco Identikey server
- Install the Vasco-server certificate on the client hosting the RES ONE Automation Agent

Please note:
* this connector is only tested with local user accounts on the Vasco Identikey Server. It is not tested with an Active Directory integrated server.
* The VascoQRurl and VascoQRshare are not used and/or tested on this moment.
* The modules are only configered for Vasco Digipasses Serials MOB30 and MOB35. But the list is easy editable to support other serials.

The following service modules are available:
- Open/Close Admin Session (all other modules already use these as first task)
- Create/Delete/List Vasco Identikey Domains
- Create/Delete/Update/List Vasco identikey Organizational Units
- List All/List first free Vasco Digipass Serials
- Assign/Unassign Vasco Digipass serial to user
- Get Digipass activation code/Get Digipass QR code (base64 image)
- Create/Delete/Update user
- Enable/Disable/Unlock user
- Reset/Set Password from user
- Reset user last authentication time
- Query User Properties

The following Run Books are available:
- List Vasco Identikey Domains
- Assign/Unassign digipass to/from user
- Create password for user
- Create/Delete user

Supporting modules:
- Get first value in the row (used in combination with List first free Vasco Digipass Serials to get only the serialnumber)
- Save Digipass QR (not used yet)
- Generate password (creates random password for first use by user)
