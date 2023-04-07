
# Platform as a service
Having a single platform to host and administer applications helps a lot! [Coolify] is a self-hostable open-source project to run such a platform. 

## Use case for Netopia
The goal is to manage all applications that are used in the future over Coolify, this way, a good overview of what is running can be ensured. 

In case that more infrastructure needs to be added due to performance reasons, this can also be configured using Coolify.

## Tech setup
Coolify holds the origin certificates for the Netopia domain, this way the included proxy can use these certificates. All the traffic generally is proxied through Cloudflare to make SSL Handling much easier.