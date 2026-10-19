# 🏥 NexPower Healthcare — Microsoft Entra ID IAM Lab

## 📌 Project Overview

This project simulates the responsibilities of an IT administrator managing Identity and Access Management (IAM) for NexPower Healthcare, a fictional healthcare organization operating a hospital and outpatient medical clinic.

Using Microsoft Entra ID Free, I created and managed a cloud-based identity environment consisting of **15 fictional user accounts**, including 14 internal employees and one third-party IT contractor. The organization uses seven security groups to organize users by business function.

The lab demonstrates hands-on experience with user provisioning, security group administration, employee account management, password resets, enterprise application assignments, and audit log monitoring.

I also configured a simulated NexPower Finance Portal enterprise application and assigned access to designated Finance employees. Because this lab uses Microsoft Entra ID Free, application assignments were performed individually rather than through security groups.

The objective of this project is to develop practical IAM and IT support administration skills while applying identity lifecycle management and least-privilege principles in a simulated business environment.

## 🎯 Project Objectives

- Provision and manage fictional employee and contractor identities using Microsoft Entra ID.
- Create department-based security groups using consistent naming conventions.
- Assign users to security groups based on their department and business responsibilities.
- Perform administrative password resets and manage user account status.
- Simulate temporary account suspension and restoration while preserving group memberships.
- Configure an enterprise application and assign designated users based on job responsibilities.
- Review audit logs to verify administrative changes and application assignments.
- Apply foundational IAM concepts, including least privilege and identity lifecycle management.

## 🛠️ Technologies & Concepts

- Microsoft Entra ID Free
- Microsoft Azure Portal
- Identity and Access Management (IAM)
- User Provisioning and Account Administration
- Security Groups and Department-Based Memberships
- Identity Lifecycle Management
- Principle of Least Privilege
- Enterprise Application User Assignments
- Audit Logs and Administrative Activity Monitoring

## 🏢 Organizational Structure

| Department | Accounts | Security Group |
|---|---:|---|
| Information Technology | 3 | SG-NPH-IT |
| Clinical Operations | 3 | SG-NPH-CLINICAL |
| Human Resources | 2 | SG-NPH-HR |
| Finance | 2 | SG-NPH-FIN |
| Sales | 2 | SG-NPH-SALES |
| Administration | 2 | SG-NPH-ADMIN |
| Contractors | 1 | SG-NPH-CONTRACTORS |
| **Total** | **15** | **7 groups** |

The organization includes employees working at the main office, medical clinic, and remotely. A third-party IT contractor is managed through a separate contractor security group.

## 📋 Project Progress

- [x] Created 15 fictional user accounts, including one third-party contractor.
- [x] Configured employee attributes, including departments, job titles, employee IDs, and office locations.
- [x] Created seven department-based security groups.
- [x] Assigned all 15 fictional accounts to their designated security groups.
- [x] Performed an administrative password reset for a test user.
- [x] Disabled and re-enabled a user account.
- [x] Verified that the user's security group membership remained intact.
- [x] Created a simulated NexPower Finance Portal enterprise application.
- [x] Assigned two Finance employees individually to the application.
- [x] Configured the application to require user assignment.
- [x] Reviewed audit logs for password resets, account changes, and application assignments.
- [x] Uploaded lab screenshots to GitHub.
- [x] Completed final README documentation and project review.

## 🔐 Hands-On IAM Exercises

### 1. User Provisioning and Identity Management

Created 15 fictional user accounts representing different departments within NexPower Healthcare.

Configured user attributes including job titles, departments, employee IDs, company affiliations, employment types, and office locations.

**Skills demonstrated:** User provisioning, identity administration, account organization, and employee record management.

### 2. Security Group Administration

Created seven security groups following a consistent `SG-NPH-` naming convention.

Assigned employees to their corresponding departmental groups and verified group memberships.

**Skills demonstrated:** Security group administration, membership management, and department-based access organization.

### 3. Password Reset Administration

Simulated an employee password recovery request involving Emily Carter from the Sales department.

Performed an administrative password reset and verified the successful operation through Microsoft Entra ID audit logs.

**Skills demonstrated:** Password administration, account recovery procedures, and audit verification.

### 4. Account Disable and Re-enable

Simulated a temporary account suspension involving Daniel Ortiz.

Disabled the user account, restored its enabled status, and verified that the employee's original security group membership remained intact.

Reviewed audit records showing changes to the `AccountEnabled` property.

**Skills demonstrated:** Account lifecycle administration, temporary access suspension, account restoration, and administrative auditing.

### 5. Enterprise Application Assignments

Created a simulated enterprise application named **NexPower Finance Portal**.

Assigned Finance employees Tom Smith and James Wilson individually and configured the application to require user assignment.

Because Microsoft Entra ID Free does not support security group-based enterprise application assignment, users were assigned individually.

**Lab limitation:** The application was not connected to a deployed Finance Portal. The exercise demonstrates application assignment configuration, not tested application sign-in or authorization enforcement.

**Skills demonstrated:** Enterprise application administration, user access assignments, and least-privilege planning.

### 6. Audit Log Monitoring

Used Microsoft Entra ID audit logs to verify the following administrative activities:

- Successful administrative password reset.
- User account disable and re-enable operations.
- Changes to the `AccountEnabled` property.
- Successful Finance Portal application assignments.

**Skills demonstrated:** Audit log review, administrative activity verification, and identity change tracking.

## 🔒 Security Considerations

This project uses fictional employee identities and simulated organizational workflows. No real patient information or production healthcare systems are involved.

The lab demonstrates foundational IAM administration and is not intended to represent a fully implemented or HIPAA-compliant healthcare environment.

Application access assignments were configured using the capabilities available in Microsoft Entra ID Free. No production application access or complete sign-in enforcement was tested.

Screenshots intended for public GitHub documentation are reviewed to avoid exposing passwords, temporary credentials, personal administrator information, and unnecessary tenant identifiers.

## 📸 Lab Documentation

The following screenshots document the IAM administration tasks completed in Microsoft Entra ID.

### 1. User and Group Administration
- [Security Groups Overview](01-Security-Groups/security-groups-overview.jpg)
- [Employee Account Directory](02-User-Accounts/employee-account-directory.jpg)

### 2. Security Group Memberships
- [IT Department Group Membership](03-Group-Memberships/it-group-membership.jpg)
- [Clinical Department Group Membership](03-Group-Memberships/clinical-group-membership.jpg)
- [Contractor Group Membership](03-Group-Memberships/contractor-group-membership.jpg)

### 3. Password and Account Management
- [Successful Password Reset](04-Password-Resets/password-reset-success.jpg)
- [User Account Disabled](05-Account-Management/user-account-disabled-Daniel.jpg)
- [User Account Re-enabled](05-Account-Management/user-account-reenabled-Daniel.jpg)

### 4. Enterprise Application Access
- [Finance Portal User Assignments](06-Access-Control/finance-app-assignments.jpg)
- [Finance Portal Assignment Requirement](06-Access-Control/finance-app-assignment-required.png)

### 5. Audit Log Verification
- [Password Reset Audit](07-Audit-Logs/password-reset-audit.jpg)
- [Account Disabled Audit](07-Audit-Logs/account-disabled-audit.jpg)
- [Account Re-enabled Audit](07-Audit-Logs/account-reenabled-audit.png)
- [Finance Application Assignment Audit](07-Audit-Logs/finance-app-assignment-audit.jpg)
  
## ✅ Project Status

**Completed — October 2026**

Successfully completed a hands-on Microsoft Entra ID IAM lab demonstrating user provisioning, security group administration, account lifecycle management, password resets, enterprise application assignments, and audit log verification.

The project includes 15 fictional identities, seven security groups, and 14 screenshots documenting the completed administrative exercises.

**Future Enhancements:** Explore Microsoft Graph PowerShell, automated user provisioning, and additional access control scenarios.
