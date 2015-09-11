# ansible-check_mk
Deploying and securely running Check_MK using worlds finest patchwork of a configuration management system. Requires *Ansible* in a rather recent version.

The role is intended for use from an OMD server, adjust group var to set the OMD site name and it'll grab the ssh key from there.

Some of most important plugins are also included for easier deployment.


Creates a service account, sets up sudo and runs Check_MK via SSH (forced command) to a dedicated user (svccmk) and sudo (restricted).


# TODO
 * Generalize / Multi OS Support
 * I use this in different versions from Sles10 to FreeBSD and it should just be one.
 * Include the caching agent and run that!
 
# questionable TODOs
 * git-/http-fetch the plugins on the executing node (since i.e. DMZ webservers might not have outgoing connectivity.)
 * Wild idea: preseed the OMD site's known hosts for all systems from ansible facts.
