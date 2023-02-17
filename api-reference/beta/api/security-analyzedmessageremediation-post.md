---
title: "Create AnalyzedMessageRemediation"
description: "Create a new microsoft.graph.security.analyzedMessageRemediation object."
author: "smkjain8"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: apiPageType
---

# Create AnalyzedMessageRemediation

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [microsoft.graph.security.analyzedMessage](../resources/security-analyzedmessage.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|SecurityAnalyzedMessage.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported|
|Application|SecurityAnalyzedMessage.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/analyzedMessageRemediations/
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body

In the request body, supply a JSON representation of the [microsoft.graph.security.analyzedMessageRemediation](../resources/security-analyzedmessageRemediation.md) object.

You can specify the following properties when creating a **analyzedMessage**.

|Property|Type|Description|
|:---|:---|:---|
|remediationName|Edm.String|The name of the remediation user wants to create.|
|severity|[microsoft.graph.security.severity](../resources/security-analyzedmessageremediation-severity.md)|The severity of remediation user wants to create. It can be low, medium and high.|
|remediationAction|[microsoft.graph.security.remediationAction](../resources/security-analyzedmessageremediation-remediationAction.md)|The admin action user wants to create.|
|description|Edm.String|The description user wants to have while creating remediation.|
|analyzedMessages|Collection([microsoft.graph.security.analyzedMessage](../resources/security-analyzedmessage.md))|The list of emails user wants to delete.|

## Response

If successful, this method returns a `201 Created` response code and a [microsoft.graph.security.analyzedMessage](../resources/security-analyzedmessage.md) object in the response body.

## Examples

### **Scenario #1 - User provides key of mail (unique identifier)**

#### Request

The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "post_analyzedMessageRemediations"
}-->
``` http
POST https://graph.microsoft.com/beta/security/analyzedMessageRemediations
Content-Type: application/json

{
    "remediationName": "SoftDelete Emails 01",
    "severity": "medium",
    "remediationAction": "softDelete",
    "description": "Emails to be soft deleted",
    "analyzedMessages": [
        {
            "id": "31ca23b8-c7b6-4f75-83dd-08daf8519e8c-15919156837756865505-1"
        }
    ]
}
```

#### Response

The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.analyzedMessageRemediation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "46a5227a-f2b3-fd21-aae1-ba0b873d0f56"
}
```

### **Scenario #2 - User provides NetworkMessageId and Recipient Email Address of mail**

#### Request

The following is an example of a request. In this scenario we create the mailmetadata key defined above at API level from both these fields but if API is called using this scenario both fields needs to be passed.

**Make sure the recipientEmailAddress is correct since it is case-sensitive.**
<!-- {
  "blockType": "request",
  "name": "post_analyzedMessageRemediations"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/analyzedMessageRemediations
Content-Type: application/json

{
    "remediationName": "SoftDelete Emails 01",
    "severity": "medium",
    "remediationAction": "softDelete",
    "description": "Emails to be soft deleted",
    "analyzedMessages": [
        {
          "networkMessageId": "8687b7c8-53cd-4009-9dad-08dae7dec99f",
          "recipientEmailAddress": "johndoe@o365tisdfv2.onmicrosoft.com"        
        }

    ]
}
```

#### Response

The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.analyzedMessageRemediation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "46a5227a-f2b3-fd21-aae1-ba0b873d0f56"
}
```

### **Scenario #3 - Both are passed**

In this scenario if both are passed, the "id" field takes precedence over other fields.

**We support both scenarios for elements defined in the analyzedMessages list. Some elements can support first scenario and others can support second scenario**
