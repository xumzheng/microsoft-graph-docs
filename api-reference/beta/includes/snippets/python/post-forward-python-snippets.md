---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ForwardPostRequestBody();
requestBody.setComment('comment-value');

toRecipientsRecipient1 = Recipient();
toRecipientsRecipient1EmailAddress = EmailAddress();
toRecipientsRecipient1EmailAddress.setName('name-value');

toRecipientsRecipient1EmailAddress.setAddress('address-value');


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress);

toRecipientsArray []= toRecipientsRecipient1;
requestBody.setToRecipients(toRecipientsArray);




await client.groupsById('group-id').threadsById('conversationThread-id').postsById('post-id').forward().post(requestBody);


```