---
title: "Get meeting transcript through Change Notifications"
description: Post meeting transcript
ms.localizationpriority: medium
author: "markwahl-msft"
ms.prod: "governance"
doc_type: "apiPageType"
---


# Get meeting transcript through Change Notifications

The document covers end-to-end flow for retrieving transcripts of Micosoft Teams meetings with [Microsoft Graph Change Notifications](https://docs.microsoft.com/en-us/graph/api/resources/webhooks?view=graph-rest-beta). Change notifications can be leveraged to get near real-time updates on meeting lifecycle events such as when a meeting transcript is ready to be viewed.

The change notifications can be subscribed at following two different levels:

* Tenant level subscription
*  User level subscription

## Tenant level subscription

Here, the app subscribes to change notifications for all the chat messages across tenant.

**Subscription resource:** [/chats/getAllMessages](https://docs.microsoft.com/en-us/graph/teams-changenotifications-chatmessage#subscribe-to-messages-across-all-chats)

Once the above subscription is created, the `notificationUrl` (specified while creating the subscription) is notified with all the different changes happening to the messages across the whole tenant.

For retrieving transcripts for meetings across the tenant, following sequence of steps can be performed:

*Note:* The payloads and response are shortened for brevity.

1. **App looks for notifications for transcription started and / or call ended notifications payload:**

	Sample Payload for Transcription Started event (event type: `callTranscriptEventMessageDetail`):

	```json
	{
		"subscriptionId": "1217470f-564c-4fe3-b51f-ebd962cb8797",
		"changeType": "created",
		"tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
		"resource": "chats('19:meeting_ZjVkMjc0ZWYtNThkMy00ZGI1LWFiYjAtYjg3ZGU0ZWI3MzZk@thread.v2')/messages('1649787549174')",
		"contentDecryptedBySimulator": {
			"@odata.context": "https://graph.microsoft.com/$metadata#chats('19%3Ameeting_ZjVkMjc0ZWYtNThkMy00ZGI1LWFiYjAtYjg3ZGU0ZWI3MzZk%40thread.v2')/messages/$entity",
			"messageType": "systemEventMessage",
			"createdDateTime": "2022-04-12T18:19:09.174Z",
			"lastModifiedDateTime": "2022-04-12T18:19:09.174Z",
			"chatId": "19:meeting_ZjVkMjc0ZWYtNThkMy00ZGI1LWFiYjAtYjg3ZGU0ZWI3MzZk@thread.v2",
			"body": {
				"contentType": "html",
				"content": "<systemEventMessage/>"
			},
			"channelIdentity": null,
			"eventDetail": {
				"@odata.type": "#Microsoft.Teams.GraphSvc.callTranscriptEventMessageDetail",
				"callId": "16481de8-3262-419b-abc7-0139e6239515",
				"callTranscriptICalUid": "",
				"meetingOrganizer": {
					"application": null,
					"device": null,
					"user": {
						"userIdentityType": "aadUser",
						"id": "14b779ae-cb64-47e7-a512-52fd50a4154d",
						"displayName": null
					}
				}
			}
		},
		"encryptedContent": {}
	}
	```

	Sample Payload for CallEnded event  (event type: `callEndedEventMessageDetail`):

	```json
	{
		"subscriptionId": "1217470f-564c-4fe3-b51f-ebd962cb8797",
		"changeType": "created",
		"tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
		"resource": "chats('19:meeting_ZjVkMjc0ZWYtNThkMy00ZGI1LWFiYjAtYjg3ZGU0ZWI3MzZk@thread.v2')/messages('1649787585457')",
		"resourceData": {},
		"contentDecryptedBySimulator": {
			"@odata.context": "https://graph.microsoft.com/$metadata#chats('19%3Ameeting_ZjVkMjc0ZWYtNThkMy00ZGI1LWFiYjAtYjg3ZGU0ZWI3MzZk%40thread.v2')/messages/$entity",
			"createdDateTime": "2022-04-12T18:19:45.457Z",
			"lastModifiedDateTime": "2022-04-12T18:19:45.457Z",		
			"chatId": "19:meeting_ZjVkMjc0ZWYtNThkMy00ZGI1LWFiYjAtYjg3ZGU0ZWI3MzZk@thread.v2",
			"eventDetail": {
				"@odata.type": "#Microsoft.Teams.GraphSvc.callEndedEventMessageDetail",
				"callId": null,
				"callDuration": "PT1M44S",
				"callEventType": "meeting",
				"callParticipants": [
				
				],
				"initiator": {
				
				}
			}
		},
		"encryptedContent": {
		
		}
	}
	```

	The app would mainly need the `chatId` property from the above payload to make subsequent calls.

**2. Get the Chat entity from ChatId ([Doc Link](https://docs.microsoft.com/en-us/graph/api/chat-get?view=graph-rest-1.0&tabs=http))**

There are two scenarios we face while retrieving chats:

  1. When the `joinWebUrl` is available in the response payload as part of the onlineMeetingInfo property.

        ``` http
        GET https://graph.microsoft.com/beta/chats/19:meeting_NmU0NTkxYzMtM2Y2My00NzRlLWFmN2YtNTFiMGM5OWM3ZjY2@thread.v2
        ```

        ```json
        {
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
            "id": "19:meeting_NmU0NTkxYzMtM2Y2My00NzRlLWFmN2YtNTFiMGM5OWM3ZjY2@thread.v2",
            "topic": "Test Meet Create Online Meeting",
            "createdDateTime": "2022-04-14T11:30:45.903Z",
            "lastUpdatedDateTime": "2022-04-26T06:27:45.265Z",
            "chatType": "meeting",
            "webUrl": "https://teams.microsoft.com/l/chat/19%3Ameeting_NmU0NTkxYzMtM2Y2My00NzRlLWFmN2YtNTFiMGM5OWM3ZjY2%40thread.v2/0?tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34",
            "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
            "viewpoint": null,
            "onlineMeetingInfo": {
                "calendarEventId": null,
                "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NmU0NTkxYzMtM2Y2My00NzRlLWFmN2YtNTFiMGM5OWM3ZjY2%40thread.v2/0?context=%7b%22Tid%22%3a%222432b57b-0abd-43db-aa7b-16eadd115d34%22%2c%22Oid%22%3a%2214b779ae-cb64-47e7-a512-52fd50a4154d%22%7d",
                "organizer": {
                    "id": "14b779ae-cb64-47e7-a512-52fd50a4154d",
                    "displayName": null,
                    "userIdentityType": "aadUser"
                }
            }
        }
        ```
  2. When the `joinWebUrl` is not available in the response. This can happen if a meeting was not created as an onlineMeeting from Teams client or was created via the Outlook client without Teams being enabled i.e. onlineMeeting switch was turned off and then the organizer edits the meeting to make it an online meeting. Online Meetings are those that are Teams-enabled. In this case, the `calendarEventId` member of the `onlineMeetingInfo` property in the response payload will be present:

        ``` http
        GET https://graph.microsoft.com/beta/chats/19:meeting_YzM1NGFiZWYtOGFiOS00NjM5LTg4OTktYmU0MjI4NTQyNGZm@thread.v2
        ```

        ```json
        {
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
            "id": "19:meeting_YzM1NGFiZWYtOGFiOS00NjM5LTg4OTktYmU0MjI4NTQyNGZm@thread.v2",
            "topic": "Non Online Meeting Teams Client",
            "createdDateTime": "2022-04-26T09:43:23.711Z",
            "lastUpdatedDateTime": "2022-04-26T09:43:46.157Z",
            "chatType": "meeting",
            "webUrl": "https://teams.microsoft.com/l/chat/19%3Ameeting_YzM1NGFiZWYtOGFiOS00NjM5LTg4OTktYmU0MjI4NTQyNGZm%40thread.v2/0?tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34",
            "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
            "viewpoint": null,
            "onlineMeetingInfo": {
                "calendarEventId": "AAMkAGE3NjJhOTVhLTNkZDQtNDE2OS05ZjU0LTJmOGQ0YTY2YTdiZQBGAAAAAAD3AG5jNnlgQJvdCL_KgXJIBwBsww5BlIxtT7iFyYWrXV3AAAAAAAENAABsww5BlIxtT7iFyYWrXV3AAACSDwYeAAA=",
                "joinWebUrl": null,
                "organizer": {
                    "id": "14b779ae-cb64-47e7-a512-52fd50a4154d",
                    "displayName": null,
                    "userIdentityType": "aadUser"
                }
            }
        }
        ```

        The `calendarEventId` property can then be used to retrieve the `joinWebUrl` by calling the calendar API ([Doc Link](https://docs.microsoft.com/en-us/graph/api/event-get?view=graph-rest-1.0&tabs=http)):

        ``` http
        GET https://graph.microsoft.com/beta/users/14b779ae-cb64-47e7-a512-52fd50a4154d/events/AAMkAGE3NjJhOTVhLTNkZDQtNDE2OS05ZjU0LTJmOGQ0YTY2YTdiZQBGAAAAAAD3AG5jNnlgQJvdCL_KgXJIBwBsww5BlIxtT7iFyYWrXV3AAAAAAAENAABsww5BlIxtT7iFyYWrXV3AAACSDwYdAAA=
        ```

        ```json
        {
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('14b779ae-cb64-47e7-a512-52fd50a4154d')/events/$entity",
            "@odata.etag": "W/\"bMMOQZSMbU+4hcmFq11dwAAAkc3Tmw==\"",
            "id": "AAMkAGE3NjJhOTVhLTNkZDQtNDE2OS05ZjU0LTJmOGQ0YTY2YTdiZQBGAAAAAAD3AG5jNnlgQJvdCL_KgXJIBwBsww5BlIxtT7iFyYWrXV3AAAAAAAENAABsww5BlIxtT7iFyYWrXV3AAACSDwYdAAA=",    
            "start": {
                "dateTime": "2022-04-26T10:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2022-04-26T11:00:00.0000000",
                "timeZone": "UTC"
            },    
            "onlineMeeting": {
                "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MTM5OTY3MGUtNmY4Mi00Yjg4LTk2MDUtY2IyZGRlNmU1ZjA2%40thread.v2/0?context=%7b%22Tid%22%3a%222432b57b-0abd-43db-aa7b-16eadd115d34%22%2c%22Oid%22%3a%2214b779ae-cb64-47e7-a512-52fd50a4154d%22%7d"
            },
            "calendar@odata.associationLink": "https://graph.microsoft.com/beta/users('14b779ae-cb64-47e7-a512-52fd50a4154d')/calendars('AAMkAGE3NjJhOTVhLTNkZDQtNDE2OS05ZjU0LTJmOGQ0YTY2YTdiZQAuAAAAAAD3AG5jNnlgQJvdCL_KgXJIAQBsww5BlIxtT7iFyYWrXV3AAAAAAAENAAA=')/$ref",
            "calendar@odata.navigationLink": "https://graph.microsoft.com/beta/users('14b779ae-cb64-47e7-a512-52fd50a4154d')/calendars('AAMkAGE3NjJhOTVhLTNkZDQtNDE2OS05ZjU0LTJmOGQ0YTY2YTdiZQAuAAAAAAD3AG5jNnlgQJvdCL_KgXJIAQBsww5BlIxtT7iFyYWrXV3AAAAAAAENAAA=')"
        }
        ```

        Here, the `onlineMeeting's` `joinUrl` property is the joinWebUrl.

**3. Get OnlineMeetingId through joinWebUrl and OrganizerId ([Doc Link](https://docs.microsoft.com/en-us/graph/api/onlinemeeting-get?view=graph-rest-1.0&tabs=http#example-3-retrieve-an-online-meeting-by-joinweburl))**

``` http
GET https://graph.microsoft.com/beta/users('14b779ae-cb64-47e7-a512-52fd50a4154d')/onlineMeetings?$filter=JoinWebUrl%20eq%20'https://teams.microsoft.com/l/meetup-join/19%3ameeting_MTM5OTY3MGUtNmY4Mi00Yjg4LTk2MDUtY2IyZGRlNmU1ZjA2%40thread.v2/0?context=%7b%22Tid%22%3a%222432b57b-0abd-43db-aa7b-16eadd115d34%22%2c%22Oid%22%3a%2214b779ae-cb64-47e7-a512-52fd50a4154d%22%7d'
```

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('14b779ae-cb64-47e7-a512-52fd50a4154d')/onlineMeetings",
    "value": [
        {
            "id": "MSoxNGI3NzlhZS1jYjY0LTQ3ZTctYTUxMi01MmZkNTBhNDE1NGQqMCoqMTk6bWVldGluZ19NVE01T1RZM01HVXRObVk0TWkwMFlqZzRMVGsyTURVdFkySXlaR1JsTm1VMVpqQTJAdGhyZWFkLnYy",
            "creationDateTime": "2022-04-26T07:41:17.3736455Z",
            "startDateTime": "2022-04-26T10:30:00Z",
            "endDateTime": "2022-04-26T11:00:00Z",
            "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MTM5OTY3MGUtNmY4Mi00Yjg4LTk2MDUtY2IyZGRlNmU1ZjA2%40thread.v2/0?context=%7b%22Tid%22%3a%222432b57b-0abd-43db-aa7b-16eadd115d34%22%2c%22Oid%22%3a%2214b779ae-cb64-47e7-a512-52fd50a4154d%22%7d",
            "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MTM5OTY3MGUtNmY4Mi00Yjg4LTk2MDUtY2IyZGRlNmU1ZjA2%40thread.v2/0?context=%7b%22Tid%22%3a%222432b57b-0abd-43db-aa7b-16eadd115d34%22%2c%22Oid%22%3a%2214b779ae-cb64-47e7-a512-52fd50a4154d%22%7d",
            "chatInfo": {
                "threadId": "19:meeting_MTM5OTY3MGUtNmY4Mi00Yjg4LTk2MDUtY2IyZGRlNmU1ZjA2@thread.v2",
                "messageId": "0",
                "replyChainMessageId": null
            }
        }
    ]
}
```

**4. Fetch Transcript through OnlineMeetingId and OrganizerId**

In the example below, *14b779ae-cb64-47e7-a512-52fd50a4154d* is the organizerId and *MSoxNGI3NzlhZS1jYjY0LTQ3ZTctYTUxMi01MmZkNTBhNDE1NGQqMCoqMTk6bWVldGluZ19ObVUwTlRreFl6TXRNMlkyTXkwME56UmxMV0ZtTjJZdE5URmlNR001T1dNM1pqWTJAdGhyZWFkLnYy* is the meetingId.

```http
GET https://graph.microsoft.com/beta/users('14b779ae-cb64-47e7-a512-52fd50a4154d')/onlineMeetings('MSoxNGI3NzlhZS1jYjY0LTQ3ZTctYTUxMi01MmZkNTBhNDE1NGQqMCoqMTk6bWVldGluZ19ObVUwTlRreFl6TXRNMlkyTXkwME56UmxMV0ZtTjJZdE5URmlNR001T1dNM1pqWTJAdGhyZWFkLnYy')/transcripts('MSMjMCMjMDEyNjJmNjgtOTc2Zi00MzIxLTlhNDQtYThmMmY4ZjQ1ZjVh')/content?$format=text/vtt
```

```webvtt
WEBVTT

0:0:0.0 --> 0:0:1.380
<v User Name>Transcription test</v>
```

## User level Subscription

Here, the app can subscribe to change notifications for calendar event of a specific user.

**Subscription resource:** [/users/\{userId\}/events](https://docs.microsoft.com/en-us/graph/outlook-change-notifications-overview?view=graph-rest-1.0)

```http

POST https://graph.microsoft.com/beta/subscriptions/
{
	"changeType": "created,updated,deleted",
	"notificationUrl": "https://tgsrelaynandanmankad.servicebus.windows.net/notifynandanmankadpc/notifications",
	"resource": "users('1273a016-201d-4f95-8083-1b7f99b3edeb')/events",
	"expirationDateTime": "2022-05-05T14:58:56.7951795+00:00",
	"clientState": "ClientSecret",
	"includeResourceData": false
}
```

1. Once the above subscription is created, the `notificationUrl` is notified with all the calendar event changes related to the user. This will send notifications when a new meeting is created. This notification will contain calendar eventId in `resource` property of the notification payload, as shown below. Here, *AAMkADY0NjM1MjRhLTNiNjAtNDBiOC1hYTQxLThkMjAxN2QzMjZhYQBGAAAAAAC03Gz8aL_JQp2Kxvw5a29SBwDFFWHjtoMRTqdrVyQ1h8yLAAAAAAENAADFFWHjtoMRTqdrVyQ1h8yLAAFwC7nAAAA=* is the `eventId`.

    ```json
    {
        "subscriptionId": "ef30cdc6-b5ae-4702-b924-f458fd9e5fc3",
        "changeType": "created",
        "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
        "clientState": "ClientSecret",
        "subscriptionExpirationDateTime": "2022-05-05T07:54:53.1886542-07:00",
        "resource": "Users/1273a016-201d-4f95-8083-1b7f99b3edeb/Events/AAMkADY0NjM1MjRhLTNiNjAtNDBiOC1hYTQxLThkMjAxN2QzMjZhYQBGAAAAAAC03Gz8aL_JQp2Kxvw5a29SBwDFFWHjtoMRTqdrVyQ1h8yLAAAAAAENAADFFWHjtoMRTqdrVyQ1h8yLAAFwC7nAAAA=",
        "resourceData": {}
    }
    ```

2. After getting the `eventId`, the app can use Get Event API to get the `JoinWebUrl` ([Doc Link](https://docs.microsoft.com/en-us/graph/api/event-get?view=graph-rest-1.0&tabs=http))

    ```http
    GET https://graph.microsoft.com/beta/users/1273a016-201d-4f95-8083-1b7f99b3edeb/events/AAMkADY0NjM1MjRhLTNiNjAtNDBiOC1hYTQxLThkMjAxN2QzMjZhYQBGAAAAAAC03Gz8aL_JQp2Kxvw5a29SBwDFFWHjtoMRTqdrVyQ1h8yLAAAAAAENAADFFWHjtoMRTqdrVyQ1h8yLAAFwC7nAAAA=
    ```
    
    ```json
    {
        "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1273a016-201d-4f95-8083-1b7f99b3edeb')/events/$entity",
        "@odata.etag": "W/\"xRVh47aDEU6na1ckNYfMiwABb2Twsg==\"",
        "id": "AAMkADY0NjM1MjRhLTNiNjAtNDBiOC1hYTQxLThkMjAxN2QzMjZhYQBGAAAAAAC03Gz8aL_JQp2Kxvw5a29SBwDFFWHjtoMRTqdrVyQ1h8yLAAAAAAENAADFFWHjtoMRTqdrVyQ1h8yLAAFwC7nAAAA=",    
        "start": {
            "dateTime": "2022-05-06T15:00:00.0000000",
            "timeZone": "UTC"
        },
        "end": {
            "dateTime": "2022-05-06T15:30:00.0000000",
            "timeZone": "UTC"
        },
    
        "onlineMeeting": {
            "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MjExYzJiMTItZDY1MS00ZGZkLWE5YzQtZTBmNWI1MDg2M2Uw%40thread.v2/0?context=%7b%22Tid%22%3a%222432b57b-0abd-43db-aa7b-16eadd115d34%22%2c%22Oid%22%3a%221273a016-201d-4f95-8083-1b7f99b3edeb%22%7d",
            "conferenceId": "438824583",
            "tollNumber": "+1 213-279-1007"
        }    
    }
    ```

3. After getting the `joinWebUrl` the app can get the `chatThreadId`, as shown in point 3 of the tenant level subscription topic.

4. Once the app has the `chatId`, it can then subscribe to get messages for a specific chat.

    **Subscription resource:** [/chats/\{chat-id\}/messages](https://docs.microsoft.com/en-us/graph/teams-changenotifications-chatmessage#subscribe-to-messages-in-a-chat)

    **OR**

    **Subscription resource:** [chats/\{chat-id\}/messages?$search=callEndedEventMessageDetail AND /chats/\{chat-id\}/messages?$search=callTranscriptEventMessageDetail](https://docs.microsoft.com/en-us/graph/teams-changenotifications-chatmessage#example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text) in case app wants subscription only for specific messages.

Once the subscription is created, the payload received for the specific chat is similar to the one seen in the tenant level subscription above in point 1.

The further process to retrieve the transcript would be exactly same as described for tenant level subscriptions in points 2 through 4.