Activiti-Designer
================

The Eclipse Mars plugin for BPMN editing

The original version of Activiti-Designer was not able to create update site for Eclipse Mars and above.
However, this was not a big thing, the designer worked well with Mars as well.

My problem was the Graphiti dependency, which was common dependecy in JPA Diagram Editor: of course the required version of Activiti-Designer for Luna(0.11.4 - @see parent project's pom) conflicted with the requred version of JPA Dialog editor (that was a different upper version) so I decided to fix it via adding Mars support to Activiti-Designer.

I had to realize (and that's why I won't create a pull request) that there was a good reason why they have not fixed it: there was some significant changes in the Graphiti API that (probably) not backward compatible.

I fixed them but I don't have the time to check the compatibility - however this fix could help someone later.

What I have checked:
- this version works well with Eclipse Mars and Oxigen
- The JPA editor and the Activiti-Designer could be installed into the same Eclipse instance



