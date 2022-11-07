- [ ] Azure app ->
Custom Domains
Find the "Custom Domain Verification ID - and copy it.

Go onto Route50
Create record
Write asuid.CHANGEME in the "Record Name"
Set the "Record Type" to TXT
Paste the Custom Domain Verification ID value into "Value".
Add another record
Write CHANGEME in the "Record Name"
Set the "Record Type" to CNAME
Copy paste the actual URL into "Value" without https://.

Go back to Custom Domains on Azure
Click on "Add custom domain"
enter CHANGEME.CHANGEMETO in "Custom Domain" and click on Validate.
Click on TLS/SSL settings
For wildcard:
Click add TLS/SSL Binding.
Chose the custom domain and the wildcard certificate.
Set "TLS/SSL Type" to SNI SSL.
For Managed:
Click on "Private Key Certificates (.pfx)
Click on "Create App Service Managed Certificate". (if you have followed the guide correctly, there will be one that is eligible)
Click on "Create"
Click on "Bindings"
Click on "Add TLS/SSL Binding"
Chose the custom domain and the created certificate.
In "TLS/SSL Type" select "SNI SSL"
