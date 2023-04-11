---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ForwardPostRequestBody()
request_body.comment = 'comment-value'

toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.name = 'name-value'

toRecipientsRecipient1EmailAddress.address = 'address-value'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
request_body.torecipients(toRecipientsArray)




request_configuration = ForwardRequestBuilderPostRequestConfiguration(
)


await client.groups_by_id('group-id').threads_by_id('conversationThread-id').posts_by_id('post-id').forward.post(request_body = request_body)


```