# NIST-800-53-project

**Overview:**

In this project, I conducted a NIST 800-53 compliance assessment by interviewing key personnel, including the CISO and IT Manager, to evaluate the organization's implementation of security controls. The assessment aimed to determine adherence to access control policies, specifically those related to least privilege (AC-6) and privileged account management.

**Objectives:**

Assess the organization's security posture regarding access control policies.

Identify compliance gaps and areas for improvement.

Provide recommendations for enhancing security controls.

Document the implementation of Azure Active Directory (AD) Role-Based Access Control (RBAC).

**Key Findings:**

**1. Implementation of Least Privilege (AC-6)**

The organization uses Microsoft Azure AD to enforce least privilege.

Normal users and administrators are assigned access only to required resources.

**2. Privileged Account Management**

Admin users manage security-relevant functions and control access permissions.

However, admin users do not utilize non-privileged accounts for routine tasks, which presents a potential security risk.

**3. Secure Network Access & Segmentation**

Authorized network access is required for privileged command execution.

The organization employs separate VLANs for HR, Finance, and IT teams to enhance security.

**4. Role-Based Access Controls (RBAC)**

Admin privileges are restricted based on roles, ensuring proper segregation of duties.

Access is granted using Azure AD permissions and role assignments.

**5. Periodic Privilege Reviews**

User privileges are reviewed periodically to ensure they are justified.

A review found that one user retained admin privileges despite a role change, prompting immediate revocation.

**6. Privileged Access Monitoring & Restrictions**

Privileged access is logged and analyzed using Azure Activity Logs.

Privileged access for non-organizational users is strictly prohibited, with guest accounts managed through Azure B2B privileged access management.

Non-privileged users cannot execute admin functions or download software without IT assistance.

**Challenges Identified:**

Admin users accessing security functions with privileged accounts instead of non-privileged accounts.

Potential risk of privilege creep due to infrequent privilege reviews.

**Recommendations:**

Implement strict enforcement of least privilege by ensuring admins use non-privileged accounts for non-security tasks.

Automate privilege review processes to detect and remove unnecessary permissions more frequently.

Strengthen privileged session monitoring to detect unauthorized access attempts proactively.

Expand the use of Multi-Factor Authentication (MFA) for privileged users.
