## AC-6: Least Privilege

### Compliance Audit

| Control Name & Identifier                                                | Finding           | Disposition            |
|--------                                                                  |----------                | ---------         |
|AC-6: Least Privilege | Enforces least privilege through RBAC. Requires access requests to be approved by by manager and the Information Security Office. Access reviews are done only annually. | *Control Partially in Place* |
|AC-6(1) Authorize Access to Security Functions                            | Uses IAM platform to control access to security functions and security-relevant information. Access to sensitive systems is restricted to members of the Security Operations Center and specific roles who need the access.| Control in Place |
|AC-6(2) Non-privileged Access for Nonsecurity Functions                   | Requires the use of non-privileged user accounts for routine business operations even for empoloyees that have privileged accounts. Enforced through system login configuration and annual trainings. | Control in Place | 
|AC-6(3) Network Access to Privileged Commands                             | Personnel can only execute privileged commands from within the corporate network or via a VPN with MFA. Policy is documented in the Network Security and Remote Access Policy.| Control in Place | 
|AC-6(4) Separate Processing Domains                                       | Currently, has two separate network segments for Finance and Engineering but full network segementation has not been fully implemented. HR lacks a network segment at the time of audit and should be prioritized due to the inherent sensitivity of employee data contained in that department.| *Control Partially In Place* | 
|AC-6(5) Privileged Accounts                                               | Requires HR and IT to designate and restrict specific employees that are allowed access to privielged accounts. Manages account provisioning through an IAM and privileged credentials are rotated and stored in password vault.| Control in Place |
|AC-6(6) Privileged Access by Non-organizational Users                     | Lacks a full standardized process for managing privileged access for non-organizational users. Currently generates access for contractors and third parties on a "case by case" basis which implies that it is manually performed. Has predominantly provided these non-organizational parties minimal access but will also temporarily grant elevated privileges for operational requirements. | *Control Partially In Place* | 
|AC-6(7) Review of User Privileges                                         | Access privileges are reviewed for all personnel on a quarterly basis. Non-organizational parties does not have a specific periodic review and are performed "ad hoc". | *Control Partially In Place* | 
|AC-6(8) Privilege Levels for Code Execution                               | User access to admin tools is blocked by default. Uses endpoint protection and application controls that prevent software from executing with elevated privileges unless approved. All applications used must be whitelisted. | Control In Place | 
|AC-6(9) Log Use of Privileged Functions                                   | Only has some logs of privileged functions via system-level logging and basic audits. Lacks consistency of logging across all systems and review is ad hoc. Critical infrastructure is scrutinized but less visibility into general privileged activity. | *Control Partially In Place* | 
|AC-6(10) Prohibit Non-privileged Users from Executing Privileged Functions| Uses RBAC to prevent non-privileged users from executing privileged functiosn on the "modern systems". Legacy systems exist and are lacking in more specific permissions controls. These legacy systems are not necessarily able to consistently enforce separation of duties. Instead relies on procedural safeguards and user training. | *Control Partially In Place* | 


### Risk Assessment

| Control Identifier| Potential Threat(s) | Vulnerability | Mitigating Factors & Compensatory Controls | Likelihood | Impact | Overall | Risk Explanation |
|-------- |----------| ---------| --------| ---------|-----| ----- | ----- |
|AC-6     | Data modification/estruction, information disclosure, unauthorized access/changes to systems   | Ex-employees or temporary contractors that were not fully offboarded could retain access to critical data and systems even after their business is complete and may not be discovered to still have this access until the annual review. | Well-established but slowly growing company. Has <20 employees currently and experiences low rates of turnover.| 5 | 10 | 50 | Risk can be reduced if access reviews are conducted more frequently (e.g. quarterly) to take into account any potential changes in personnel or third parties contractors. |
|AC-6(1) | - | - | -| - | - | - | -|
|AC-6(2) | - | - | -| - | - | - | - |
|AC-6(3) | - | - | -| - | - | - | - |
|AC-6(4) | Information disclosure, unauthorized access/changes to systems | content | content| 2 | 8 | 16 | content |
|AC-6(5) | - | - | -| - | - | - | -|
|AC-6(6) | content | content | content| content | content | content | content |
|AC-6(7) | content | content | content| content | content | content | content |
|AC-6(8) | - | - | -| - | - | - | - |
|AC-6(9) | content | content | content| content | content | content | content |
|AC-6(10) | content | content | content| content | content | content | content |
