[this document is a draft of the API documentation to be uploaded to Github]

**Namespace**

Security

&gt; Audit Search

&gt; Overview

&gt; Audit Log Query

&gt; List

&gt; Get

&gt; Create

&gt; List Audit Log Records

## **Overview**

Page Title: Use the Microsoft Graph Audit Search API

The Microsoft Graph APIs for Audit Search provide functionality for organizations to automate repetitive tasks involving retrieval of Audit records. For details about searching the Audit log, see [Search the audit log in the Microsoft Purview compliance portal](https://learn.microsoft.com/en-us/microsoft-365/compliance/audit-log-search?view=o365-worldwide).

The Audit Search API is defined in the subnamespace microsoft.graph.security. The API includes the following key entities.

| **Name** | **Type** | **Use case** |
| --- | --- | --- |
| Audit Log Query | Microsoft.graph.security.auditLogQuery | <br> |
| Audit Log Record | Microsoft.graph.security.auditLogRecord | <br> |

## **Audit Log Query**

Namespace: microsoft.graph.security.auditCore

AuditLogQuery describes the query entity created by tenant-admin.

## **Methods**

| Method | Return type | Description |
| --- | --- | --- |
| <br> | <br> | <br> |
| <br> | <br> | <br> |
| <br> | <br> | <br> |
| <br> | <br> | <br> |

## **Properties**

| <br> | <br> | <br> | <br> |
| --- | --- | --- | --- |
| <br> | <br> | <br> | <br> |
| <br> | <br> | <br> | <br> |
| <br> | <br> | <br> | <br> |
| <br> | <br> | <br> | <br> |
| <br> | <br> | <br> | <br> |

## **Relationships**

| <br> | <br> | <br> |
| --- | --- | --- |
| <br> | <br> | <br> |

## **&gt; List**

Namespace: microsoft.graph.security

(One line to explain what the API does. E.g.: Get the list of AuditLogQuery entities created.)

## **Permissions**

Through the Audit Search Graph API, auditing data can be accessed using the following permissions which are classified at a workload level. To learn more, including how to choose permissions, see [Microsoft Graph permissions reference](https://learn.microsoft.com/en-us/graph/permissions-reference).

| **Permission type** | **Permissions** | **Description** |
| --- | --- | --- |
| Delegated | AuditLogsQueryAAD.Read.All | Audit records that belong to AzureActiveDirectory workload |
| <br> | AuditLogsQueryCRM.Read.All | Audit records that belong to CRM workload |
| <br> | AuditLogsQueryEndpoint.Read.All | Audit records that belong to Endpoint workload |
| <br> | AuditLogsQueryExchange.Read.All | Audit records that belong to Exchange workload |
| <br> | AuditLogsQueryOneDrive.Read.All | Audit records that belong to OneDrive workload |
| <br> | AuditLogsQuerySharePoint.Read.All | Audit records that belong to SharePoint workload |
| <br> | AuditLogsQueryGeneral.Read.All | Audit records that belong to all **other** workloads not listed above (does not grant access to the above listed workloads) |
| <br><br>Application | AuditLogsQueryAAD.Read.All | Audit records that belong to AzureActiveDirectory workload |
| <br> | AuditLogsQueryCRM.Read.All | Audit records that belong to CRM workload |
| <br> | AuditLogsQueryEndpoint.Read.All | Audit records that belong to Endpoint workload |
| <br> | AuditLogsQueryExchange.Read.All | Audit records that belong to Exchange workload |
| <br> | AuditLogsQueryOneDrive.Read.All | Audit records that belong to OneDrive workload |
| <br> | AuditLogsQuerySharePoint.Read.All | Audit records that belong to SharePoint workload |
| <br> | AuditLogsQueryGeneral.Read.All | Audit records that belong to all **other** workloads not listed above (does not grant access to the above listed workloads) |

## **Request**

(describe request structure here)

## **Response**

(describe response structure here)

## **Examples**

**Request**

The following is an example of a request.

[add example request]

**Response**

The following is an example of the response.

Note: The response object shown here might be shortened for readability.

[add example response]

## **&gt; Get**

Namespace: microsoft.graph.security

(One line to explain what the API does.)

## **Permissions**

Through the Audit Search Graph API, auditing data can be accessed using the following permissions which are classified at a workload level. To learn more, including how to choose permissions, see [Microsoft Graph permissions reference](https://learn.microsoft.com/en-us/graph/permissions-reference).

| **Permission type** | **Permissions** | **Description** |
| --- | --- | --- |
| Delegated | AuditLogsQueryAAD.Read.All | Audit records that belong to AzureActiveDirectory workload |
| <br> | AuditLogsQueryCRM.Read.All | Audit records that belong to CRM workload |
| <br> | AuditLogsQueryEndpoint.Read.All | Audit records that belong to Endpoint workload |
| <br> | AuditLogsQueryExchange.Read.All | Audit records that belong to Exchange workload |
| <br> | AuditLogsQueryOneDrive.Read.All | Audit records that belong to OneDrive workload |
| <br> | AuditLogsQuerySharePoint.Read.All | Audit records that belong to SharePoint workload |
| <br> | AuditLogsQueryGeneral.Read.All | Audit records that belong to all **other** workloads not listed above (does not grant access to the above listed workloads) |
| <br><br>Application | AuditLogsQueryAAD.Read.All | Audit records that belong to AzureActiveDirectory workload |
| <br> | AuditLogsQueryCRM.Read.All | Audit records that belong to CRM workload |
| <br> | AuditLogsQueryEndpoint.Read.All | Audit records that belong to Endpoint workload |
| <br> | AuditLogsQueryExchange.Read.All | Audit records that belong to Exchange workload |
| <br> | AuditLogsQueryOneDrive.Read.All | Audit records that belong to OneDrive workload |
| <br> | AuditLogsQuerySharePoint.Read.All | Audit records that belong to SharePoint workload |
| <br> | AuditLogsQueryGeneral.Read.All | Audit records that belong to all **other** workloads not listed above (does not grant access to the above listed workloads) |

## **Request**

(describe request structure here)

## **Response**

(describe response structure here)

## **Examples**

**Request**

The following is an example of a request.

[add example request]

**Response**

The following is an example of the response.

Note: The response object shown here might be shortened for readability.

[add example response]

## **&gt; Create**

Namespace: microsoft.graph.security

(One line to explain what the API does.)

## **Permissions**

Through the Audit Search Graph API, auditing data can be accessed using the following permissions which are classified at a workload level. To learn more, including how to choose permissions, see [Microsoft Graph permissions reference](https://learn.microsoft.com/en-us/graph/permissions-reference).

| **Permission type** | **Permissions** | **Description** |
| --- | --- | --- |
| Delegated | AuditLogsQueryAAD.Read.All | Audit records that belong to AzureActiveDirectory workload |
| <br> | AuditLogsQueryCRM.Read.All | Audit records that belong to CRM workload |
| <br> | AuditLogsQueryEndpoint.Read.All | Audit records that belong to Endpoint workload |
| <br> | AuditLogsQueryExchange.Read.All | Audit records that belong to Exchange workload |
| <br> | AuditLogsQueryOneDrive.Read.All | Audit records that belong to OneDrive workload |
| <br> | AuditLogsQuerySharePoint.Read.All | Audit records that belong to SharePoint workload |
| <br> | AuditLogsQueryGeneral.Read.All | Audit records that belong to all **other** workloads not listed above (does not grant access to the above listed workloads) |
| <br><br>Application | AuditLogsQueryAAD.Read.All | Audit records that belong to AzureActiveDirectory workload |
| <br> | AuditLogsQueryCRM.Read.All | Audit records that belong to CRM workload |
| <br> | AuditLogsQueryEndpoint.Read.All | Audit records that belong to Endpoint workload |
| <br> | AuditLogsQueryExchange.Read.All | Audit records that belong to Exchange workload |
| <br> | AuditLogsQueryOneDrive.Read.All | Audit records that belong to OneDrive workload |
| <br> | AuditLogsQuerySharePoint.Read.All | Audit records that belong to SharePoint workload |
| <br> | AuditLogsQueryGeneral.Read.All | Audit records that belong to all **other** workloads not listed above (does not grant access to the above listed workloads) |

## **Request**

(describe request structure here)

## **Response**

(describe response structure here)

## **Examples**

**Request**

The following is an example of a request.

[add example request]

**Response**

The following is an example of the response.

Note: The response object shown here might be shortened for readability.

[add example response]

## **&gt; List Audit Log Record**

Namespace: microsoft.graph.security

AuditLogRecord is returned for a query based on the query filters provided in the AuditLogQuery entity. This is openType as the schema would be different for different workloads, operations and auditLogRecordTypes.

The schemas for each workload are described here: https://learn.microsoft.com/en-us/office/office-365-management-api/office-365-management-activity-api-schema#auditlogrecordtype

Auditing platform allows workloads to push auditLogRecords in their custom schema and AuditQuery allows the query on the customer schema attributes.

## **Methods**

| Method | Return type | Description |
| --- | --- | --- |
| <br> | <br> | <br> |
| <br> | <br> | <br> |
| <br> | <br> | <br> |
| <br> | <br> | <br> |

## **Properties**

| <br> | <br> | <br> | <br> |
| --- | --- | --- | --- |
| <br> | <br> | <br> | <br> |
| <br> | <br> | <br> | <br> |
| <br> | <br> | <br> | <br> |
| <br> | <br> | <br> | <br> |
| <br> | <br> | <br> | <br> |

## **Relationships**

| <br> | <br> | <br> |
| --- | --- | --- |
| <br> | <br> | <br> |

## **Permissions**

Through the Audit Search Graph API, auditing data can be accessed using the following permissions which are classified at a workload level. To learn more, including how to choose permissions, see [Microsoft Graph permissions reference](https://learn.microsoft.com/en-us/graph/permissions-reference).

| **Permission type** | **Permissions** | **Description** |
| --- | --- | --- |
| Delegated | AuditLogsQueryAAD.Read.All | Audit records that belong to AzureActiveDirectory workload |
| <br> | AuditLogsQueryCRM.Read.All | Audit records that belong to CRM workload |
| <br> | AuditLogsQueryEndpoint.Read.All | Audit records that belong to Endpoint workload |
| <br> | AuditLogsQueryExchange.Read.All | Audit records that belong to Exchange workload |
| <br> | AuditLogsQueryOneDrive.Read.All | Audit records that belong to OneDrive workload |
| <br> | AuditLogsQuerySharePoint.Read.All | Audit records that belong to SharePoint workload |
| <br> | AuditLogsQueryGeneral.Read.All | Audit records that belong to all **other** workloads not listed above (does not grant access to the above listed workloads) |
| <br><br>Application | AuditLogsQueryAAD.Read.All | Audit records that belong to AzureActiveDirectory workload |
| <br> | AuditLogsQueryCRM.Read.All | Audit records that belong to CRM workload |
| <br> | AuditLogsQueryEndpoint.Read.All | Audit records that belong to Endpoint workload |
| <br> | AuditLogsQueryExchange.Read.All | Audit records that belong to Exchange workload |
| <br> | AuditLogsQueryOneDrive.Read.All | Audit records that belong to OneDrive workload |
| <br> | AuditLogsQuerySharePoint.Read.All | Audit records that belong to SharePoint workload |
| <br> | AuditLogsQueryGeneral.Read.All | Audit records that belong to all **other** workloads not listed above (does not grant access to the above listed workloads) |

## **Request**

(describe request structure here)

## **Response**

(describe response structure here)

## **Examples**

**Request**

The following is an example of a request.

[add example request]

**Response**

The following is an example of the response.

Note: The response object shown here might be shortened for readability.

[add example response]