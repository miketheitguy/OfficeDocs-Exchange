---
title: 'Database Availability Groups role: Exchange 2013 Help'
TOCTitle: Database Availability Groups role
ms:assetid: 0b3e0f7a-21e5-4209-8d5b-b63c6b9de3cc
ms:mtpsurl: https://technet.microsoft.com/library/Dd876847(v=EXCHG.150)
ms:contentKeyID: 49289157
ms.reviewer: 
ms.topic: article
manager: serdars
description: About the Database Availability Groups management role in Microsoft Exchange
ms.author: serdars
author: msdmaguire
f1.keywords:
- NOCSH
mtps_version: v=EXCHG.150
---

# Database Availability Groups role

_**Applies to:** Exchange Server 2013_

The `Database Availability Groups` management role enables administrators to manage database availability groups in an organization. Administrators assigned this role either directly or indirectly are the highest level administrators responsible for the high availability configuration in an organization.

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
|[Organization Management](organization-management-exchange-2013-help.md)|X|X|`Organization`|`Organization`|`OrganizationConfig`|`OrganizationConfig`|
