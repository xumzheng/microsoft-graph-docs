---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ForwardPostRequestBody()
request_body.setComment('comment-value')

toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.setName('name-value')

toRecipientsRecipient1EmailAddress.setAddress('address-value')


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress)

toRecipientsArray []= toRecipientsRecipient1;
request_body.setToRecipients(toRecipientsArray)




await client.groups_by_id('group-id').threads_by_id('conversationThread-id').posts_by_id('post-id').forward.post(request_body, headers=)


```