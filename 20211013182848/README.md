# Active Directory 
 
User management utility. 
Widely used.

Microsoft True Ops to help evaluate *potential* costs 
 
User forest
  - Can contain multiple domains
  - We use single domain forest, likely the most common type of domain forest 
  - OU (Organizational Units)
    - *Users* and *Computers* is the dedault OUs 
      - We try *not* to use Users
    - Can be nested 
    - Inherit from parents (by default)
    - GPO (Group Policy Object)
      - More flexible/restrictive Do's/Don't 
    - SvcAccts 
      - accounts for internal services
      - require additional restrictions

AWS uses *managed AD* 
  - AWSADmin is the highest level we can escalate in AWS_AD
  - restrictions 
    - 
  - managed by AWS 
  - Delegated groups to get around  lack of things like Enterprise Admins

We use Azure AD 
providing less pain points than full ADFS setup on prem/ on our own
- Authentication that Mircosoft SErvices are built on
- Roles instead of security groups 
  - built in roles
  - domain admin = global administrator


SAML is a snowflake. All providers are different

PLuralsight AD stuff /AzureAD


RAS Remote Auth Service

Enterprise admins
None of the following are available in AWS AD
  not used for D2D
schema
  AD schema controls
Domain
   domain user
    d2d
  azure admin 
  
Active Directory Federation Services (ADFS)
  - LDAP built into AD 
 

IEP (Identity ? ?) 

portal.azure.com 
needs full domain name. ad.fedramp.gov... check console docs.
