# Answers to Assignment 8 Part 3

Add your answers to the questions in Assignment 8 Part 3, Step 2 below. 

## Vulernability Remediation:
### Vulnerability 1: 
1. Which package or library are you addressing?
Package: PyYAML
2. Which CVE is linked to this vulnerability?
CVE-2019-20477
3. What remediation steps do you suggest?
Upgrade to a version that contains a fix for this - or for mitigation purposes use yaml.safe_load` or the SafeLoader loader when you parse untrusted input. - From https://access.redhat.com/security/cve/cve-2019-20477

### Vulnerability 2:
1. Which vulnerability are you addressing?
OsPackageVulnerability
2. Which CVE is linked to this vulnerability?
CVE-2020-14343
3. What remediation steps do you suggest? 
Use a vetted library or framework that does not allow this weakness to occur or provides constructs that make this weakness easier to avoid
Ensure that you perform input validation at well-defined interfaces within the application. This will help protect the application even if a component is reused or moved elsewhere
Assume all input is malicious. Use an “accept known good” input validation strategy, i.e., use a list of acceptable inputs that strictly conform to specifications. Reject any input that does not strictly conform to specifications, or transform it into something that does.
From https://avd.aquasec.com/nvd/2019/cve-2019-14343/