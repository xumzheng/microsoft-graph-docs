---
title: "educationAssignment: setUpResourcesFolder"
description: "Create a SharePoint folder to upload files for a given educationAssignment."
ms.localizationpriority: medium
author: "sharmas"
ms.prod: "education"
doc_type: apiPageType
---

# educationAssignment: setUpResourcesFolder

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a SharePoint folder to upload files for a given [educationAssignment](../resources/educationassignment.md). 

The teacher determines the resources to upload in the assignment's folder. 

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) |  EduAssignments.ReadBasic, EduAssignments.Read  |
|Delegated (personal Microsoft account) |  Not supported.  |
|Application | Not supported. | 

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/setUpResourcesFolder
```
## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |
| Content-Type   | application/json. Required. |

## Request body
In the request body, supply an empty JSON object `{}` for this method.

## Response
If successful, this method returns a `200 OK` response code and an [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) object in the request body.

If the specified **assignment** already has a folder, this method returns a `400 Bad request` and an error response.

## Example
The following example shows how to call this API.

### Request
The following is an example of a request.



# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["d38ffdea-da93-46ac-90ba-d568c6073075","ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],  
  "name": "educationassignment_setupresourcesfolder"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/education/classes/b07edbef-7420-4b3d-8f7c-d599cf21e069/assignments/1e5222bd-b7d2-4d64-8a22-74b722ce2fc6/submissions/803fb5dd-3553-455f-3d94-f79fb54a1003/setUpResourcesFolder
Content-type: application/json

{
}
```
# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-setupresourcesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-setupresourcesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-setupresourcesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-setupresourcesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---
### Response
The following is an example of the response. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('1e5222bd-b7d2-4d64-8a22-74b722ce2fc6')/submissions/$entity",
    "status": "working",
    "submittedDateTime": null,
    "unsubmittedDateTime": null,
    "returnedDateTime": null,
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2",
    "id": "803fb5dd-3553-455f-3d94-f79fb54a1003",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1",
            "displayName": null
        }
    },
    "unsubmittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "returnedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "resources": [],
    "submittedResources": []
}
-->

