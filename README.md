<!-- Generated by Build-ReadmeFromPowerShellHelp -->
# Get-ExpiringAdfsCertificate
This script will query AD FS certificates (via Get-AdfsCertficate) and Relying Party Trust certificates (via Get-AdfsRelyingPartyTrust) and check if the certificates expire within a user-defined threshold (or the default 30 days if not specified). It will then output details about expiring certificates, and,  optionally, send an alert email.

## Getting Started
<!-- Build-ReadmeFromPowerShellHelp GettingStarted Section Start -->
Enter Getting Started Info Here
<!-- Build-ReadmeFromPowerShellHelp GettingStarted Section End -->

### Prerequisites
<!-- Build-ReadmeFromPowerShellHelp Prerequisites Section Start -->
Enter Prerequisite Info Here
<!-- Build-ReadmeFromPowerShellHelp Prerequisites Section End -->

### Installing
<!-- Build-ReadmeFromPowerShellHelp Installing Section Start -->
Enter Installation Info Here
<!-- Build-ReadmeFromPowerShellHelp Installing Section End -->

## Usage
### Examples
```PowerShell
.\Get-ExpiringAdfsCertificate.ps1
CertType            Name                                        ExpiryDate
--------            ----                                        ----------
RP Trust Encryption app.fabrikam.com                            2/14/2018 8:31:43 AM
RP Trust Signing    app.fabrikam.com                            2/14/2018 8:31:43 AM
ADFS                CN=ADFS Encryption - adfs.treyresearch.net  11/12/2018 2:15:12 PM
ADFS                CN=ADFS Signing - adfs.treyresearch.net     11/12/2018 2:15:13 PM
```
```PowerShell
.\Get-ExpiringAdfsCertificate.ps1 -EmailFrom adfs@treyresearch.net -EmailTo noc@treyresearch.net -SmtpServer mail.treyresearch.net -SmtpAuthenticated -NoOutput
(Does not generate an output, but emails details about expiring certificates to noc@treyresearch.net)
```
### Documentation
<!-- Build-ReadmeFromPowerShellHelp Documentation Section Start -->
For detailed documentation, consult [Get-ExpiringAdfsCertificate.ps1.md](../blob/master/Get-ExpiringAdfsCertificate.ps1.md) or run Get-Help Get-ExpiringAdfsCertificate.ps1 in PowerShell.
<!-- Build-ReadmeFromPowerShellHelp Documentation Section End -->

## Questions/Comments
<!-- Build-ReadmeFromPowerShellHelp Questions Section Start -->
If you have questions, comments, etc, please enter a GitHub Issue with the "question" tag.
<!-- Build-ReadmeFromPowerShellHelp Questions Section End -->

## Contributing/Bug Reporting
<!-- Build-ReadmeFromPowerShellHelp Contributing Section Start -->
Contributions and bug reports are gladly accepted! Please see (CONTRIBUTING.md)[../blob/master/CONTRIBUTING.md] for details.
<!-- Build-ReadmeFromPowerShellHelp Contributing Section End -->

## Authors
<!-- Build-ReadmeFromPowerShellHelp Authors Section Start -->
**AUTHORNAMEHERE** - *Initial work* - [GITHUBUSERNAMEHERE](https://github.com/GITHUBUSERNAMEHERE)
<!-- Build-ReadmeFromPowerShellHelp Authors Section End -->

## License
<!-- Build-ReadmeFromPowerShellHelp License Section Start -->
This project is licensed under LICENSEINFOHERE - see [LICENSE.md](../blob/master/LICENSE.md) for details.
<!-- Build-ReadmeFromPowerShellHelp License Section End -->

## Acknowledgements
<!-- Build-ReadmeFromPowerShellHelp Acknowledgements Section Start -->
Enter Acknowledgements Here
<!-- Build-ReadmeFromPowerShellHelp Acknowledgements Section End -->


