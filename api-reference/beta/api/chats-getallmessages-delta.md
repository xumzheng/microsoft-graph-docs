---
title: "chats: getAllMessages/delta"
description: "Get incremental changes for messages from all chats that a user is a participant in."
author: "DiegoCont"
ms.localizationpriority: high
ms.prod: "microsoft-teams"
doc_type: apiPageType
---

# chats: getAllMessages/delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get incremental changes for all messages from all [chats](../resources/chatmessage.md) that a user is a participant in, including one-on-one chats, group chats, and meeting chats.

[!INCLUDE [teams-model-A-and-B-disclaimer](../../includes/teams-model-A-and-B-disclaimer.md)]

## Permissions

The following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account)| Not supported |
|Delegated (personal Microsoft account) | Not supported |
|Application | Chat.Read.All, Chat.ReadWrite.All |

> [!NOTE]
> Before calling this API with application permissions, you must request access. For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).

## HTTP request

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | user-principal-name}/chats/getAllMessages/delta
```

## Optional query parameters
You can use `model` query parameter, which supports the values `A` and `B`, based on the preferred [licensing and payment model](/graph/teams-licenses),
as shown in the following examples.  
If no `model` is specified, [evaluation mode](/graph/teams-licenses#evaluation-mode-default-requirements) will be used.

```http
GET /users/{id | user-principal-name}/chats/getAllMessages/delta?model=A
GET /users/{id | user-principal-name}/chats/getAllMessages/delta?model=B
```

`$top` parameter is configurable only at the start of the synchronization. If this parameter is included in subsequent requests, new value will be ignored and the original one will be used instead.

```http
GET /users/{id}/chats/getAllMessages/delta?$top=50
 ```

There is limited support for `$filter` parameter. The only supported $filter expression is `$filter=lastModifiedDateTime+gt+{value}`.

```http
GET /users/{id}/chats/getAllMessages/delta?$top=50&$filter=lastModifiedDateTime gt 2020-06-04T18:03:11.591Z
 ```
 `$orderby` parameter is not supported. The return order of items is not guaranteed; default ordering is `DESC` but `updated` and `deleted` items take priority over pending items.

## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required. |

## Response

If successful, this method returns a `200 OK` response code and a list of [chatMessages](../resources/chatmessage.md) in the response body as well as a @odata.nextLink (that contains a URL with a delta function call and a skipToken), or a @odata.deltaLink (that contains a URL with a delta function call and deltaToken).
  
These tokens are state tokens that are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the URL returned from the last GET request to the next delta function call for the same user. A @odata.deltaLink returned in a response signifies that the current round of change tracking is complete. You can save and use the @odata.deltaLink URL when you begin the next round.

>**Note:** State tokens expire after 7 days if not used.
  
## Example

The following example shows two rounds of synchronization

### First Request

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages/delta?$top=2
```

### Response

The response includes two messages and an @odata.nextLink response header. The @odata.nextLink URL indicates there are more pending messages
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
   "@odata.nextLink":"https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages/delta?$skiptoken=JiRkC2_stNeLP2UCGBwIsfp0R3KXLikR9MrIeZrEzwfr4JXHJf6mDyqxSpdnG_Mmj8IQL1KherBjJDZuqEoxm8TfuIMDQJHCvAa4LvNK1jVHgtmiljuPcKKG6ydmQk5vLDlFHLOAH_jrUTfeUhh7gwh8JwVY3DgLslb0J31BFLMP9tMLoMSXAtBDSE0i9vCVu7qcv-45YNtKozlvPKg36gOgS8FwDMvv9msKMC7DmJZKUrelSmfNhCEV-eGk7N0kMLTAcc9RpKAWDRwzlS66QV2SMXcS0gWAQHvdKimKbCS__aUDIBzyozCxC9cW_NQi829VUt5SGlbKrphOX82GAOcl8g6Jeef5uQvkxpwDe1UrI-IW9DUg2gh4Vt3CyFzqqAX5NzeQmANhqAdOwedmWOc-4ETB7ZsJLa3UUa8PjoTZDGwhxBHLZvjlCysRIlEg.5pdLXOWF_W4hm_tia96yeaFrviXuQajWr-ASwnr5jEQ",
   "value":[
      {
         "@odata.type":"#microsoft.graph.chatMessage",
         "id":"1600457965467",
         "replyToId":null,
         "etag":"1600457965467",
         "messageType":"message",
         "createdDateTime":"2020-09-18T19:39:25.467Z",
         "lastModifiedDateTime":"2020-09-18T19:39:25.467Z",
         "lastEditedDateTime":null,
         "deletedDateTime":null,
         "subject":null,
         "summary":null,
         "chatId":"19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_5c64e248-3269-4268-a36e-0f80314e9c39@unq.gbl.spaces",
         "importance":"normal",
         "locale":"en-us",
         "webUrl":null,
         "channelIdentity":null,
         "policyViolation":null,
         "eventDetail": null,
         "from":{
            "application":null,
            "device":null,
            "conversation":null,
            "user":{
               "id":"0de69e5e-2da8-4cf2-821f-5e6585b2c65b",
               "displayName":"Richard Wilson",
               "userIdentityType":"aadUser"
            }
         },
         "body":{
            "contentType":"html",
            "content":"<div>\n<blockquote itemscope=\"\" itemtype=\"http://schema.skype.com/Reply\" itemid=\"1600457867820\">\n<strong itemprop=\"mri\" itemid=\"8:orgid:0de69e5e-2da8-4cf2-821f-5e6585b2c65b\">Richard Wilson</strong><span itemprop=\"time\" itemid=\"1600457867820\"></span>\n<p itemprop=\"preview\">1237</p>\n</blockquote>\n<p>this is a reply</p>\n</div>"
         },
         "attachments":[

         ],
         "mentions":[

         ],
         "reactions":[

         ]
      }
   ]
}
```
  ### Second Request

The second request specifies the @odata.nextLink URL returned from the previous response.
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages/delta?$skiptoken=JiRkC2_stNeLP2UCGBwIsfp0R3KXLikR9MrIeZrEzwfr4JXHJf6mDyqxSpdnG_Mmj8IQL1KherBjJDZuqEoxm8TfuIMDQJHCvAa4LvNK1jVHgtmiljuPcKKG6ydmQk5vLDlFHLOAH_jrUTfeUhh7gwh8JwVY3DgLslb0J31BFLMP9tMLoMSXAtBDSE0i9vCVu7qcv-45YNtKozlvPKg36gOgS8FwDMvv9msKMC7DmJZKUrelSmfNhCEV-eGk7N0kMLTAcc9RpKAWDRwzlS66QV2SMXcS0gWAQHvdKimKbCS__aUDIBzyozCxC9cW_NQi829VUt5SGlbKrphOX82GAOcl8g6Jeef5uQvkxpwDe1UrI-IW9DUg2gh4Vt3CyFzqqAX5NzeQmANhqAdOwedmWOc-4ETB7ZsJLa3UUa8PjoTZDGwhxBHLZvjlCysRIlEg.5pdLXOWF_W4hm_tia96yeaFrviXuQajWr-ASwnr5jEQ
```
 
 ### Response
 The second response returns the remaining messages and a @odata.deltaLink URL which indicates synchronization is complete for the time being. Save and use the @odata.deltaLink URL to synchronize the messages in the next round.
  
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
   "@odata.deltaLink":"https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages/delta?$deltatoken=JiRkC2_stNeLP2UCGBwIsfp0R3KXLikR9MrIeZrEzwfr4JXHJf6mDyqxSpdnG_Mmj8IQL1KherBjJDZuqEoxm8TfuIMDQJHCvAa4LvNK1jVHgtmiljuPcKKG6ydmQk5vLDlFHLOAH_jrUTfeUhh7gwh8JwVY3DgLslb0J31BFLMP9tMLoMSXAtBDSE0i9vCVu7qcv-45YNtKozlvPKg36gOgS8FwDMvv9msKMC7DmJZKUrelSmfNhCEV-eGk7N0kMLTAcc9RpKAWDRwzlS66QV2SMXcS0gWAQHvdKimKbCS__aUDIBzyozCxC9cW_NQi829VUt5SGlbKrphOX82GAOcl8g6Jeef5uQvkxpwDe1UrI-IW9DUg2gh4Vt3CyFzqqAX5NzeQmANhqAdOwedmWOc-4ETB7ZsJLa3UUa8PjoTZDGwhxBHLZvjlCysRIlEg.5pdLXOWF_W4hm_tia96yeaFrviXuQajWr-ASwnr5jEQ",
   "value":[
      {
         "@odata.type":"#microsoft.graph.chatMessage",
         "id":"1600457965467",
         "replyToId":null,
         "etag":"1600457965467",
         "messageType":"message",
         "createdDateTime":"2020-09-18T19:39:25.467Z",
         "lastModifiedDateTime":"2020-09-18T19:39:25.467Z",
         "lastEditedDateTime":null,
         "deletedDateTime":null,
         "subject":null,
         "summary":null,
         "chatId":"19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_5c64e248-3269-4268-a36e-0f80314e9c39@unq.gbl.spaces",
         "importance":"normal",
         "locale":"en-us",
         "webUrl":null,
         "channelIdentity":null,
         "policyViolation":null,
         "eventDetail": null,
         "from":{
            "application":null,
            "device":null,
            "conversation":null,
            "user":{
               "id":"0de69e5e-2da8-4cf2-821f-5e6585b2c65b",
               "displayName":"Richard Wilson",
               "userIdentityType":"aadUser"
            }
         },
         "body":{
            "contentType":"html",
            "content":"<div>\n<blockquote itemscope=\"\" itemtype=\"http://schema.skype.com/Reply\" itemid=\"1600457867820\">\n<strong itemprop=\"mri\" itemid=\"8:orgid:0de69e5e-2da8-4cf2-821f-5e6585b2c65b\">Richard Wilson</strong><span itemprop=\"time\" itemid=\"1600457867820\"></span>\n<p itemprop=\"preview\">1237</p>\n</blockquote>\n<p>this is a reply</p>\n</div>"
         },
         "attachments":[

         ],
         "mentions":[

         ],
         "reactions":[

         ]
      }
   ]
}
```
  ### Third Request

The third request specifies the @odata.deltaLink URL returned from the previous response.
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages/delta?$deltatoken=JiRkC2_stNeLP2UCGBwIsfp0R3KXLikR9MrIeZrEzwfr4JXHJf6mDyqxSpdnG_Mmj8IQL1KherBjJDZuqEoxm8TfuIMDQJHCvAa4LvNK1jVHgtmiljuPcKKG6ydmQk5vLDlFHLOAH_jrUTfeUhh7gwh8JwVY3DgLslb0J31BFLMP9tMLoMSXAtBDSE0i9vCVu7qcv-45YNtKozlvPKg36gOgS8FwDMvv9msKMC7DmJZKUrelSmfNhCEV-eGk7N0kMLTAcc9RpKAWDRwzlS66QV2SMXcS0gWAQHvdKimKbCS__aUDIBzyozCxC9cW_NQi829VUt5SGlbKrphOX82GAOcl8g6Jeef5uQvkxpwDe1UrI-IW9DUg2gh4Vt3CyFzqqAX5NzeQmANhqAdOwedmWOc-4ETB7ZsJLa3UUa8PjoTZDGwhxBHLZvjlCysRIlEg.5pdLXOWF_W4hm_tia96yeaFrviXuQajWr-ASwnr5jEQ)
```
  
  ### Response
   Third Response containing @odata.deltaLink and empty body
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
   "@odata.deltaLink":"https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages/delta?$deltatoken=JiRkC2_stNeLP2UCGBwIsfp0R3KXLikR9MrIeZrEzwfr4JXHJf6mDyqxSpdnG_Mmj8IQL1KherBjJDZuqEoxm8TfuIMDQJHCvAa4LvNK1jVHgtmiljuPcKKG6ydmQk5vLDlFHLOAH_jrUTfeUhh7gwh8JwVY3DgLslb0J31BFLMP9tMLoMSXAtBDSE0i9vCVu7qcv-45YNtKozlvPKg36gOgS8FwDMvv9msKMC7DmJZKUrelSmfNhCEV-eGk7N0kMLTAcc9RpKAWDRwzlS66QV2SMXcS0gWAQHvdKimKbCS__aUDIBzyozCxC9cW_NQi829VUt5SGlbKrphOX82GAOcl8g6Jeef5uQvkxpwDe1UrI-IW9DUg2gh4Vt3CyFzqqAX5NzeQmANhqAdOwedmWOc-4ETB7ZsJLa3UUa8PjoTZDGwhxBHLZvjlCysRIlEg.5pdLXOWF_W4hm_tia96yeaFrviXuQajWr-ASwnr5jEQ",
   "value":[]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chats: getallmessages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
