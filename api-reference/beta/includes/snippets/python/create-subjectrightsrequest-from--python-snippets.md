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

request_body.includeAllVersions = false

request_body.includeAuthoredContent = true

request_body.internalDueDateTime = DateTime('2022-07-20T22:42:28Z')

dataSubject = DataSubject()
dataSubject.firstName = 'Diego'

dataSubject.lastName = 'Siciliani'

dataSubject.email = 'Diego.Siciliani@contoso.com'

dataSubject.residency = 'USA'


request_body.dataSubject = dataSubject
request_body.mailboxLocations=null

request_body.pauseAfterEstimate = true

request_body.Regulations(['CCPA', ])

siteLocations = SubjectRightsRequestSiteLocation()
siteLocations.@odatatype = 'microsoft.graph.subjectRightsRequestAllSiteLocation'


request_body.siteLocations = siteLocations
approversUser1 = User()
approversUser1.id = '1B761ED2-AA7E-4D82-9CF5-C09D737B6167'


approversArray []= approversUser1;
request_body.approvers(approversArray)




request_configuration = SubjectRightsRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.privacy.subjectRightsRequests.post(request_body = request_body)


```