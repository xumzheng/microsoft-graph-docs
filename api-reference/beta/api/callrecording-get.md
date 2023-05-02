---
title: "Get callRecording"
description: "Retrieve a single callRecording associated with a Microsoft Teams online meeting."
author: "v-sdhakshina"
ms.localizationpriority: medium
ms.prod: "microsoft-teams"
doc_type: apiPageType
---

# Get callRecording

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retrieve a [callRecording](../resources/callrecording.md) object associated with an [onlineMeeting](../resources/onlinemeeting.md).

Retrieving the recording returns the metadata of the single recording associated with the online meeting. Retrieving the content of the recording returns the stream of text associated with the recording.

> **Notes:** 
> - In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.
> - This API works differently in one or more national clouds. For details, see [Implementation differences in national clouds](/graph/teamwork-national-cloud-differences). 

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | OnlineMeetingRecording.Read.All |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | OnlineMeetingRecording.Read.All |

To use application permission for this API, tenant administrators must create an application access policy and grant it to a user. This authorizes the app configured in the policy to fetch online meetings and/or online meeting artifacts on behalf of that user (with the user ID specified in the request path). For more details, see [Allow applications to access online meetings on behalf of a user](/graph/cloud-communication-online-meeting-application-access-policy).

> [!NOTE]
> This API works for a meeting only if the meeting has not expired. For more details, see [Limits and specifications for Microsoft Teams](/microsoftteams/limits-specifications-teams#meeting-expiration).

## HTTP request

<!-- { "blockType": "ignored" } -->

Get a single recording of an online meeting.

```http
GET /me/onlineMeetings/{meetingId}/recordings/{recordingId}
GET /users/{userId}/onlineMeetings/{meetingId}/recordings/{recordingId}
```

Get the content of a single recording of an online meeting.

```http
GET me/onlineMeetings/{meetingId}/recordings/{recordingId}/content
GET users/{userId}/onlineMeetings/{meetingId}/recordings/{recordingId}/content
```

## Request headers

| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [callRecording](../resources/callRecording.md) object in the response body.

## Examples

> [!NOTE]
> The docx format for recordings will be deprecated starting May 31, 2023.

### Example 1: Get a callRecording
#### Request

# [HTTP](#tab/http)

``` http
GET https://graph.microsoft.com/beta/users/ba321e0d-79ee-478d-8e28-85a19507f456/onlineMeetings/MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ/recordings/MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4
```

---

#### Response

> **Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callrecording"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('ba321e0d-79ee-478d-8e28-85a19507f456')/onlineMeetings('MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ')/recordings/$entity",
    "id": "MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4",
    "createdDateTime": "2021-09-17T06:09:24.8968037Z"
}
```

### Example 2: Get a callRecording content
#### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecording_content",
  "sampleKeys": ["ba321e0d-79ee-478d-8e28-85a19507f456", "MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ", "MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4"]
}
-->
``` http
GET https://graph.microsoft.com/beta/users/ba321e0d-79ee-478d-8e28-85a19507f456/onlineMeetings/MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ/recordings/MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4/content
```

---

#### Response

Response contains bytes for the recording in the body. `content-type` header specifies type of the recording content. Negative offsets indicate that the recordingion began while the conversation was ongoing.

>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
}
-->
```http
HTTP/1.1 200 OK
Content-type: text/vtt

WEBVTT

0:0:0.0 --> 0:0:5.320
<v User Name>This is a recording test.</v>
```

### Example 3: Get a callRecording content specifying $format query param
#### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callRecording_content_format",
  "sampleKeys": ["ba321e0d-79ee-478d-8e28-85a19507f456", "MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ", "MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4"]
}
-->
``` http
GET https://graph.microsoft.com/beta/users/ba321e0d-79ee-478d-8e28-85a19507f456/onlineMeetings/MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ/recordings/MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4/content?$format=text/vtt
```

---

#### Response

Response contains bytes for the recording in the body. `content-type` header specifies type of the recording content.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
}
-->
```http
HTTP/1.1 200 OK
Content-type: text/vtt

WEBVTT

0:0:0.0 --> 0:0:5.320
<v User Name>This is a recording test.</v>
```

### Example 4: Get a callRecording content specifying Accept header

>**Note:** The docx format and `Accept` header will be deprecated starting May 31, 2023.

#### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callRecording_content_Accept",
  "sampleKeys": ["ba321e0d-79ee-478d-8e28-85a19507f456", "MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ", "MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4"]
}
-->
``` http
GET https://graph.microsoft.com/beta/users/ba321e0d-79ee-478d-8e28-85a19507f456/onlineMeetings/MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ/recordings/MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4/content
Accept: application/vnd.openxmlformats-officedocument.wordprocessingml.document
```

---

#### Response

Response contains bytes for the recording in the body. `Content-Type` header specifies type of the recording content.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/vnd.openxmlformats-officedocument.wordprocessingml.document

0:0:0.0 --> 0:0:5.320
User Name
This is a recording test.
```
### Example 5: Get a callRecording content with $format getting precedence over the Accept header

>**Note:** The docx format and `$format` query parameter will be deprecated starting May 31, 2023.

#### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecording_content_format_precedence",
  "sampleKeys": ["ba321e0d-79ee-478d-8e28-85a19507f456", "MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ", "MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4"]
}
-->
``` http
GET https://graph.microsoft.com/beta/users/ba321e0d-79ee-478d-8e28-85a19507f456/onlineMeetings/MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ/recordings/MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4/content?$format=text/vtt
Accept: application/vnd.openxmlformats-officedocument.wordprocessingml.document
```

---

#### Response

Response contains bytes for the recording in the body. `Content-Type` header specifies type of the recording content.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
}
-->
```http
HTTP/1.1 200 OK
Content-type: text/vtt

WEBVTT

0:0:0.0 --> 0:0:5.320
<v User Name>This is a recording test.</v>
```

### Example 6: Get a callRecording metadataContent
#### Request
# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callRecording_metadatacontent"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/ba321e0d-79ee-478d-8e28-85a19507f456/onlineMeetings/MSo1N2Y5ZGFjYy03MWJmLTQ3NDMtYjQxMy01M2EdFGkdRWHJlQ/recordings/MSMjMCMjNzU3ODc2ZDYtOTcwMi00MDhkLWFkNDItOTE2ZDNmZjkwZGY4/metadataContent
```

---

#### Response
> **Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
}
-->
```http
HTTP/1.1 200 OK
Content-type: text/vtt

WEBVTT

00:00:16.246 --> 00:00:17.726
{"startDateTime":"2023-03-08T08:22:30.0461639+00:00","endDateTime":"2023-03-08T08:22:31.5261639+00:00","speakerName":"User Name","spokenText":"This is a transcription test.","spokenLanguage":"en-us"}
```
