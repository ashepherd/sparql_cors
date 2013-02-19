To support Javascript and web applications querying a Drupal SPARQL endpoint, 
this module implements CORS (http://www.w3.org/TR/cors/) to support cross-domain 
requests.This module currently supports GET requests against the /sparql menu 
path from the sparql_endpoint module (http://drupal.org/project/sparql). 

There is a configuration form for this module that lets a user with the 
'administer administration pages' permission to specify a list of domains that 
should be allowed to make cross-domain requests to the SPARQL endpoint. However, 
requests from these domains must provide an 'Origin' header in the request. All 
domains can be enabled by speciyfing '*' as a domain.

For more information, see http://enable-cors.org/