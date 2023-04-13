---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SubjectRightsRequest()
request_body.Type(SubjectRightsRequestType('export'))

request_body.contentQuery = '((\"Diego Siciliani\" OR \"Diego.Siciliani@contoso.com\") OR (participants:\"Diego.Siciliani@contoso.com\"))'

request_body.DataSubjectType(DataSubjectType('customer'))

request_body.externalId = 'F53BF2DA-607D-412A-B568-FAA0F023AC0B'

request_body.displayName = 'Export report for customer Id: 12345'

request_body.description = 'This is a export request'

request_body.include_all_versions = False

request_body.include_authored_content = True

request_body.internalDueDateTime = DateTime('2022-07-20T22:42:28Z')

data_subject = DataSubject()
dataSubject.firstName = 'Diego'

dataSubject.lastName = 'Siciliani'

dataSubject.email = 'Diego.Siciliani@contoso.com'

dataSubject.residency = 'USA'


request_body.data_subject = dataSubject
request_body.mailboxLocations=null

request_body.pause_after_estimate = True

request_body.Regulations(['CCPA', ])

site_locations = SubjectRightsRequestSiteLocation()
siteLocations.@odatatype = 'microsoft.graph.subjectRightsRequestAllSiteLocation'


request_body.site_locations = siteLocations
approvers_user1 = User()
approversUser1.id = '1B761ED2-AA7E-4D82-9CF5-C09D737B6167'


approversArray []= approversUser1;
request_body.approvers(approversArray)





result = await client.privacy.subjectRightsRequests.post(request_body = request_body)


```