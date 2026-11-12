# Microsoft Entra ID – Conditional Access MFA Demonstration

## Project Overview

This project demonstrates the implementation of a Microsoft Entra ID Conditional Access policy designed to strengthen identity security by requiring Multi-Factor Authentication (MFA) for selected users accessing Office 365.

The project follows Zero Trust security principles by applying identity-based access controls and evaluating authentication requirements before policy enforcement.

## Objectives

- Implement Conditional Access in Microsoft Entra ID.
- Create a dedicated security group for test users.
- Configure MFA as an access requirement.
- Target selected cloud applications.
- Evaluate policy behaviour using Report-only mode.
- Understand sign-in monitoring and Conditional Access evaluation.

## Tools and Technologies

- Microsoft Entra ID
- Microsoft Azure
- Conditional Access
- Multi-Factor Authentication (MFA)
- Office 365
- Microsoft Entra Sign-in Logs

## Implementation

### 1. Security Group Creation

Created a dedicated security group:

`GRP-CA-MFA-TestUsers`

This group provides a controlled population for testing Conditional Access policies.

### 2. Conditional Access Policy

Policy name:

`CA001-Require-MFA-TestUsers`

### 3. Policy Configuration

| Configuration | Setting |
|---|---|
| Users and groups | GRP-CA-MFA-TestUsers |
| Target resources | Office 365 |
| Network | Not configured |
| Conditions | Not configured |
| Grant control | Require multifactor authentication |
| Session controls | Not configured |
| Policy state | Report-only |

### 4. Report-only Mode

The policy was created in Report-only mode to evaluate its potential impact without enforcing the configured access requirements.

This allows administrators to review policy behaviour before moving to enforcement.

### 5. Sign-in Monitoring

Test sign-in activity was generated using a cloud-only test account.

Microsoft Entra Sign-in Logs provide visibility into authentication activity and Conditional Access policy evaluation.

The specific evaluation result for the new policy should be verified before claiming successful policy evaluation.

## Security Principles Demonstrated

- Identity and Access Management (IAM)
- Multi-Factor Authentication
- Least Privilege
- Zero Trust Security
- Controlled Policy Deployment
- Cloud Identity Protection

## Project Evidence

Screenshots and demonstration recordings are included to document the configuration process.

## Key Learning Outcomes

This project provided practical experience in configuring Microsoft Entra Conditional Access, assigning policies to selected users, targeting cloud applications, and understanding Report-only policy evaluation.

## Future Improvements

- Verify Conditional Access evaluation results.
- Test MFA enforcement after controlled policy activation.
- Implement location-based Conditional Access.
- Explore device-based access controls.
- Investigate sign-in risk and user risk policies.

## Disclaimer

This is a controlled learning environment created for educational and portfolio demonstration purposes. The policy remains in Report-only mode and has not been presented as an enforced production security control.

---

**Author:** Oni Victor Kehinde

**Focus Areas:** Cloud Security | Identity and Access Management | Microsoft Entra ID | SOC Operations
