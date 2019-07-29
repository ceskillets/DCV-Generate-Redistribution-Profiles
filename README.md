# RedistProfileSkillet
This Skillet creates redistribution profiles for routing protocols in PANOS

Sometimes a Palo Alto Networks firewall need to participate in routing with the existing network infrastructure.  Redistribution Profiles allow security admins to share prefix information between different routing protocols. If a route was learned from a routing protocol such as OSPF and need to be advertised from BGP a redistribution profile is the configuration option that is needed to achieve that goal.

Redistribution Profiles are configured under the firewall’s Virtual Router, which is typically defined as “default”.  Redistribution profiles identify which routes you want to redistribute into another routing protocol.

This skillet will have you identify the source of the prefix (e.g. how it was learned), and the specific prefixes you would like to specifically add to the profile.

# panhandler application
This skillet is designed to be used with the panhandler application to API load structured configurations.

panhandler (at https://panhandler.readthedocs.io)

# Support Policy
The code and templates in the repo are released under an as-is, best effort, support policy. These scripts should be seen as community supported and Palo Alto Networks will contribute our expertise as and when possible. We do not provide technical support or help in using or troubleshooting the components of the project through our normal support options such as Palo Alto Networks support teams, or ASC (Authorized Support Centers) partners and backline support options. The underlying product used (the VM-Series firewall) by the scripts or templates are still supported, but the support is only for the product functionality and not for help in deploying or using the template or script itself. Unless explicitly tagged, all projects or work posted in our GitHub repository (at https://github.com/PaloAltoNetworks) or sites other than our official Downloads page on https://support.paloaltonetworks.com are provided under the best effort policy.
