---
title: "Create analyzedMessageRemediation"
description: "Create a new analyzedMessageRemediation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: apiPageType
---

# Create analyzedMessageRemediation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [analyzedMessageRemediation](../resources/analyzedmessageremediation.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|Mail.ReadWrite|
|Delegated (personal Microsoft account)|Not supported|
|Application|Mail.ReadWrite	|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST analyzedMessageRemediations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the RemediationRequest object.

You can specify the following properties when creating an **RemediationRequest**.

|Property|Type|Description|
|:---|:---|:---|
|remediationName|String|The name of the remediation user wants to create.|
|severity|String|The severity of remediation user wants to create. It can be low, medium and high.|
|type|String|The admin action user wants to create. It can be SoftDelete, HardDelete, MoveToInbox and MoveToJunk|
|description|String|The description user wants to have while creating remediation.|
|analyzedMessages|[Collection(Value)](../resources/analyzedmessageremediation.md)|The description user wants to have while creating remediation.|



## Response

If successful, this method returns a `200 Created` response code and an [analyzedMessageRemediation](../resources/analyzedmessageremediation.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "create_analyzedmessageremediation_from_analyzedmessageremediations"
}
-->
``` http
POST https://graph.microsoft.com/beta/analyzedMessageRemediations
Content-Type: application/json
Content-length: 355

{
	"remediationName": "SoftDelete Emails 01",
	"severity": "medium",
	"type": "SoftDelete",
	"description": "Emails to be soft deleted",
	"analyzedMessages": {
		"@odata.context": "https://graph.microsoft.com/v1.0/$metadata#/security/analyzedMessage",
		"value": [
			{
				"id": "6e41e872-9e46-46cd-700a-08d9990ddb14-16737038841889323262-1"
			}
		]
	}
}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.analyzedMessageRemediation"
}
-->
``` http
HTTP/1.1 200 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.analyzedMessageRemediation",
  "id": "3f0e78a8-f94d-a87d-db3b-960469428a7e",
  "bulkId": "2b09ed57-662c-47c5-9d47-4b920748b208"
}
```

