# A simple application for Medical Diagnostic Devices

This is a simplified model for an application intended to manage the configuration of medical devices for an organization working in the Clinical [In-vitro Diagnotic](http://en.wikipedia.org/wiki/In_vitro_diagnostics) Market. 

The samples are taken from the company [bioMerieux Inc](www.biomerieux.com), based in the RTP Area in NC.


## Resources

The main resource of the application is a medical system. A System is an instrument that the company installs on customer sites (hospital, labs, medical and clinical centers) to perform in-vitro diagnostic tests.  
These systems are built with a number of parts or components, which are also represented in this model as a resource. Any instrument system may have one or several components attached to them. 
The goal of this application is to allow an instrument administrator in the organization to keep track of all the systems supported by the different business units or areas, and the composition of these systems, that is, all the components defined for each of them. 

## Resource: Instrument Systems 
This is the main resource of the application, the following information is kept for each system:
**System ID:** It is the key attribute that identifies the system in the organization. It is a seven-character code with for format: **XXX9999**. The first three letters identify the type of instrument and the last 4 digits specify the capacity (number of tests or samples that can be executed in one single run). For instance: BTA0120, BTA0240, VTK0060.

**Name:** The commercial brand name of the system.

**Country of Origin:** three-letter code of the country from the manufacturer, the options are: USA, France, China, Brazil and Italy; locations where the organization has the manufacturing plants. 

**Application:** It is the product line or areas where the systems are applied, for instance Bacteriology, Cancers, Virology, and others.

**Product Manager:** Name of the organization's employee in charge of the technical support and operations for the system. 

**Image:** A picture of the system. Pictures can be taken from the company website. 

**Corporate Website:** A link to the library of products and instruments maintained by the organization in their public websites. 


## Resource: Equipment Components
Parts used to build an instrument system. Attributes:

**Name:** The brand name of the product. 

**Part Type:** To specify whether the part is required for the system, or it is an optional component. 

**Component Status:** The status of a given component could be "Active" or "Obsolete".

A piece of equipment defined as  a component can be used in one or several systems. 


## Application Flow and use cases. 
The instrument base administrator should be able to create a system in the application and add as many components as required to complete the configuration. 
If the Product Manager determines that a component should no longer be included in a system, the application should allow to set the status of this component as obsolete. 

The solution should let the user to search and filter instrument systems by "Country of Origin" or "Application". 

For Components, users should be able to search and filter by "Component Name" and by "Status".

## Metadata Annotations
Systems and components are annotated with microdata, using terms defined in Schema.org 

Systems and Components are defined as extensions of the Schema.org term: Product, as
 
 schema.org/Product/Clinical/Diagnostic/System
 
 schema.org/Product/Clinical/Diagnostic/Component
 

For Systems:
The property "Country of Origin" is annotated through the terms "Organization/Corporation", "PostalAddress" and "Country".

The property "application" is also an extension of the Product's property "brand". 

A property "productManager" is created for the term Product. The property is linked to the class "Person", using the standard property "name".




 

