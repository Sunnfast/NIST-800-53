# NIST 800-53 AC-6: Least Privilege Questionnaire

Company: Nine Houses

CISO: John Gaius
IT Director: Pyrrha Dve

**AC-6: How does your organization implement least privilege? How does your organization ensure that users only have access to the data that are necessary to accomplish assigned organizational tasks?**

> Nine Houses enforces least privilege through a role-based access control (RBAC) model, aligned with job functions and responsibilities. Access requests must be approved by both the employee’s manager and the Information Security Office. Access is granted based only on what is required for users to perform their organizational duties. Periodic access reviews are conducted quarterly to ensure access remains appropriate.

**AC-6(1): How does your organization authorize access for specific individuals or roles to perform organization-defined:**

**Security functions (deployed in hardware, software, and firmware); and**

**Security-relevant information?**

> Access to security functions and security-relevant information is authorized via our Identity and Access Management (IAM) platform, which is integrated with HR workflows. Security administrators assign access based on predefined roles, and access to sensitive systems (e.g., intrusion detection, audit logs) is limited to members of the Security Operations Center (SOC) or specific engineering roles with documented need.

**AC-6(2): Does your organization have a policy that requires users of system accounts or roles with access to security functions use non-privileged accounts when accessing nonsecurity functions?**

> Yes. Nine Houses mandates that users with privileged accounts also maintain separate, non-privileged user accounts for routine business operations. This policy is outlined in our Acceptable Use and Privilege Access Policy, and enforced through system login configurations and user education.

**AC-6(3): Does your organization have a policy that requires authorized network access in order to use privileged commands? If so, where is this policy documented?**

> Yes. Privileged commands can only be executed from within the corporate network or via secure VPN with multifactor authentication. This requirement is documented in the Network Security and Remote Access Policy, which is reviewed annually by the Information Security Office.

**AC-6(4): Does your organization have separate network domains for different departments within the organization that ensures that departments only have access to the information they need?**

> Nine Houses is in the process of developing more formalized network segmentation across departments. Currently, there is some logical separation of systems—particularly for Finance and Engineering—but not all departments have dedicated network domains. Access to sensitive data is primarily controlled through application-level permissions rather than network-level segmentation. We are working toward a more robust model that aligns with least privilege principles as part of our infrastructure roadmap.

**AC-6(5): How does your organization restrict the use of privileged accounts to designated personnel or roles?**

>Privileged accounts are restricted to designated personnel and roles as defined by HR and IT leadership. Account provisioning is managed through a centralized IAM system, and privileged credentials are rotated regularly and stored securely in a password vault. All administrative access is logged and monitored.

**AC-6(6): How does your organization prevent non-organizational users from obtaining privileged access?** 

**How is this achieved?**

> Currently, Nine Houses does not have a fully standardized process for managing privileged access for non-organizational users. In practice, access for contractors or third parties is granted on a case-by-case basis, often coordinated between department heads and IT. While such users are typically granted limited access, there are instances where elevated privileges may be temporarily assigned for operational needs. We recognize the need for tighter controls and are evaluating tools and processes to better restrict and monitor privileged access for non-employees.

**AC-6(7): Does your organization periodically review the privileges assigned to users to verify if they are still necessary? Does your organization reassign or remove privileges if access is no longer necessary for organizational business and mission needs?**

> Yes. Access privileges are reviewed quarterly as part of our user access review process. Managers receive reports on user entitlements and must attest to their continued necessity. Any unnecessary privileges are promptly revoked, and terminated users are deprovisioned within 24 hours.

**AC-6(8): Does your organization have controls in place to prevent software from executing at a higher privilege level than users executing the software?**

>Yes. Nine Houses uses endpoint protection and application control solutions that prevent software from running with elevated privileges unless explicitly approved. Applications must be digitally signed and whitelisted before execution. User access to administrative tools is blocked by default.

**AC-6(9): Does your organization log the use of privileged functions?**

> Nine Houses does capture some logs related to the use of privileged functions, primarily through system-level logging and basic audit trails. However, logging is not yet consistent across all systems, and the review of these logs is largely ad hoc. While critical infrastructure is monitored more closely, broader visibility into privileged activity is an area we know needs improvement, and plans are underway to centralize and automate log collection and review.

**AC-6(10): Does your organization have controls in place to prevent non-privileged users from executing privileged functions?**

> Nine Houses enforces role-based access controls to prevent non-privileged users from executing privileged functions on most modern systems. However, some legacy systems used by certain departments lack granular permission controls and make it more difficult to enforce strict separation of duties. In those cases, we rely on procedural safeguards and user training to mitigate risk, though we acknowledge this is not ideal. We are currently evaluating options to phase out or better isolate these legacy systems to bring them in line with our broader security standards.
