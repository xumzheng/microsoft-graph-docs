---
title: "Delete retentionEventType"
description: "Deletes a retentionEventType object."
author: "sseth"
ms.localizationpriority: medium
ms.prod: "compliance"
doc_type: apiPageType
---

# Delete retentionEventType
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delete a [retentionEventType](../resources/security-retentioneventtype.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|RecordsManagement.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|RecordsManagement.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /security/labels/retentionLabels/{retentionLabelId}/eventType/$ref
DELETE /security/triggerTypes/retentionEventTypes/{retentionEventTypeId}/$ref
DELETE /security/triggers/retentionEvents/{retentionEventId}/retentionEventType/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_retentioneventtype"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/security/triggerTypes/retentionEventTypes/{retentionEventTypeId}
```

# [powershellv1](#tab/powershellv1)
[!INCLUDE [sample-code](../includes/snippets/powershellv1/delete-retentioneventtype-powershellv1-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [powershellv2](#tab/powershellv2)
[!INCLUDE [sample-code](../includes/snippets/powershellv2/delete-retentioneventtype-powershellv2-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### Response
>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

