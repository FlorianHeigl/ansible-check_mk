# ansible-check_mk
Deploying and securely running Check_MK using worlds finest patchwork of a configuration management system. Requires Ansible in a rather recent version.


Creates a service account, sets up sudo and runs Check_MK via SSH (forced command) and sudo (restricted).


# TODO
 * Generalize / Multi OS Support
 * I use this in different versions from Sles10 to FreeBSD and it should
just be one.
 * Include the caching agent and run that!
