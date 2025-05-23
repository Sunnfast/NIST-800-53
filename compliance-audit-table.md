## AC-6: Least Privilege

### Compliance Audit

| Control Name & Identifier                                                | Finding           | Disposition            |
|--------                                                                  |----------                | ---------         |
|AC-6(1) Authorize Access to Security Functions                            | Enforces least privilege through RBAC. Requires access to be approved by by manager and the Information Security Office. Uses IAM platform to control access to security functions and security-relevant information. Access to sensitive systems is restricted to members of the Security Operations Center and specific roles who need the access.| Control in Place |
|AC-6(2) Non-privileged Access for Nonsecurity Functions                   | Requires the use of non-privileged user accoutns for routine business operations even for empoloyees that have privileged accounts. Enforced through system login configuration and annual trainings. | Control in Place | 
|AC-6(3) Network Access to Privileged Commands                             | Personnel can only execute privileged commands from within the corporate network or via a VPN with MFA. Policy is documented in the Network Security and Remote Access Policy.| Control in Place | 
|AC-6(4) Separate Processing Domains                                       | Currently, has two separate network segments for Finance and Engineering but full network segementation has not been fully implemented. HR lacks a network segment at the time of audit and should be prioritized due to the inherent sensitivity of employee data contained in that department.| *Control Partially In Place* | 
|AC-6(5) Privileged Accounts                                               | Requires HR and IT to designate and restrict specific employees that are allowed access to privielged accounts. Manages account provisioning through an IAM and privileged credentials are rotated and stored in password vault.| Control in Place |
|AC-6(6) Privileged Access by Non-organizational Users                     | Lacks a full standardized process for managing privileged access for non-organizational users. Currently generates access for contractors and third parties on a "case by case" basis which implies that it is manually performed. Has predominantly provided these non-organizational parties minimal access but will also temporarily grant elevated privileges for operational requirements. | *Control Partially In Place* | 
|AC-6(7) Review of User Privileges                                         | content | Control In Place | 
|AC-6(8) Privilege Levels for Code Execution                               | content | Control In Place | 
|AC-6(9) Log Use of Privileged Functions                                   | content | *Control Partially In Place* | 
|AC-6(10) Prohibit Non-privileged Users from Executing Privileged Functions| content | *Control Partially In Place* | 


### Risk Assessment

| Control Identifier| Potential Threat(s) | Vulnerability | Mitigating Factors |  Compensatory Controls| Likelihood | Impact | Overall | Risk Explanation |
|-------- |----------| ---------| --------| ---------|-----| ----- | ----- | ------ |
|AC-6(1) | content | content | content| content | content |
|AC-6(2) | content | content | content| content | content |
|AC-6(3) | content | content | content| content | content |
|AC-6(4) | content | content | content| content | content |
|AC-6(5) | content | content | content| content | content |
|AC-6(6) | content | content | content| content | content |
|AC-6(7) | content | content | content| content | content |
|AC-6(8) | content | content | content| content | content |
|AC-6(9) | content | content | content| content | content |
|AC-6(10) | content | content | content| content | content |
