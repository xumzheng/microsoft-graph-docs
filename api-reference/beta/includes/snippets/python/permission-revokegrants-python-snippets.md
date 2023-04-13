---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RevokeGrantsPostRequestBody()
grantees_drive_recipient1 = DriveRecipient()
granteesDriveRecipient1.email = 'ryan@contoso.com'


granteesArray []= granteesDriveRecipient1;
request_body.grantees(granteesArray)





result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').permissions_by_id('permission-id').revokeGrants.post(request_body = request_body)


```