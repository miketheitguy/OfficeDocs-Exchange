---
title: 'ApplicationImpersonation role: Exchange 2013 Help'
TOCTitle: ApplicationImpersonation role
ms:assetid: d6e43a2f-9b1f-463e-8c56-ca38d9127a5a
ms:mtpsurl: https://technet.microsoft.com/library/Dd776119(v=EXCHG.150)
ms:contentKeyID: 49289425
ms.topic: article
ms.reviewer: 
manager: serdars
ms.author: serdars
author: msdmaguire
f1.keywords:
- NOCSH
mtps_version: v=EXCHG.150
description: "Information about the ApplicationImpersonation role."
---

# ApplicationImpersonation role

_**Applies to:** Exchange Server 2013_

The `ApplicationImpersonation` management role enables applications to impersonate users in an organization to perform tasks on behalf of the user.

For example, you might see these roles in the Exchange admin center:

- ISVMailboxUsers\_\<xxxxx\>
- RIM-MailboxAdmins\<xxxxxxxxxx\>

> [!IMPORTANT]
> A process or application that's a member of the <CODE>ApplicationImpersonation</CODE> role can access the contents of a user's mailbox and act on behalf of that user, even if the user's account is disabled. This might let users access their mailboxes if you have applications, like Blackberry Enterprise Server, that use the <CODE>ApplicationImpersonation</CODE> role. Third-party products that don't use the <CODE>ApplicationImpersonation</CODE> role and instead use Exchange ActiveSync can't access a mailbox after its user account has been disabled.<BR>To prevent an application that uses the <CODE>ApplicationImpersonation</CODE> role from accessing a mailbox or performing tasks on its behalf after its user account has been disabled, do one or more of the following:
> <UL>
> <LI>
> <P>Disable or remove the user in the third-party application.</P>
> <LI>
> <P>Delete the mailbox.</P></LI></UL>

## Default management role assignments

This role has role assignments to one or more role assignees. The following table indicates whether the role assignment is regular or delegating, and also indicates the management scopes applied to each assignment. The following list describes each column:

- **Regular assignment**: Regular role assignments enable the role assignee to access the permissions provided by the management role entries on this role.
- **Delegating assignment**: Delegating role assignments give the role assignee the ability to assign this role to role groups, users, or USGs.
- **Recipient read scope**: The recipient read scope determines what recipient objects the role assignee is allowed to read from Active Directory.
- **Recipient write scope**: The recipient write scope determines what recipient objects the role assignee is allowed to modify in Active Directory.
- **Configuration read scope**: The configuration read scope determines what configuration and server objects the role assignee is allowed to read from Active Directory.
- **Configuration write scope**: The configuration write scope determines what organizational and server objects the role assignee is allowed to modify in Active Directory.

### Default management role assignments for this role

|Role group|Regular assignment|Delegating assignment|Recipient read scope|Recipient write scope|Configuration read scope|Configuration write scope|
|---|:---:|:---:|---|---|---|---|
|[Hygiene Management](hygiene-management-exchange-2013-help.md)||X|`Organization`|`Organization`|`None`|`None`|
|[Organization Management](organization-management-exchange-2013-help.md)||X|`Organization`|`Organization`|`None`|`None`|
