---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Set_status_message_post_request_body()
status_message = Presence_status_message()
status_messagemessage = Item_body()
status_messagemessage.content = 'Hey I\'m currently in a meeting.'

status_messagemessage.contenttype(BodyType.Text('bodytype.text'))


status_message.message = status_messagemessage
status_messageexpiry_date_time = Date_time_time_zone()
status_messageexpiry_date_time.date_time = '2022-10-18T17:05:33.2079781'

status_messageexpiry_date_time.time_zone = 'Pacific Standard Time'


status_message.expiry_date_time = status_messageexpiry_date_time

request_body.status_message = status_message



await client.users.by_user_id('user-id').presence.set_statu_message.post(request_body = request_body)


```