# VendorDetails
Yaml Files describing specific details of vendor software to aid understanding and investigation

##
Currently experimenting with this as an idea, I don't know if this has been done somewhere else. I'm hoping this could be used for documenting details of products as well as their dependencies to aid investigations and understanding.

I think this could be done as part of internal development as well as externally. I'm not a software developer at all, so again maybe there's additional fields which could be of utility. 

Current fields:

id: An ID field for this particular version

vendor name: Self explanatory, may not be a "vendor" per-se, but it should best describe who "owns" it for maintenance

product name: Self explanatory

product version: v1.9

author: Martin Connarty

product description:
- A quick description of what the product does and its purpose, and maybe a bit about how it works. I have found this can be difficult to determine sometimes and have had to trawl through websites to find this.

version description: 
- Any particular details or changes that were introduced to the version

dependency hash: 
- An MD5 hash of the various dependencies listed below, not sure how needed this is so may remove this field

dependencies: 
  - A list of IDs of other products that this depends on
  
known_domains:
  - Domains that this is know to communicate to, in order to confirm legitimate traffic

known_ips:
  - IP addreses this is known to communicate to, again in order to help confirm legitimate traffic

user_agents:
  - Any known user agents that this uses

registry_keys:
  - All of the known registry key locations

process_names:
  - Names of the processes you are likely to see

imphashes:
  - Import hashes of these processes

logging details:
  - Details of where logs may be found and what they log

vulnerabilities:
  - Details of any known vulnerabilities
