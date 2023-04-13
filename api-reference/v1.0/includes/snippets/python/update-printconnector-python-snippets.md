---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrintConnector()
request_body.displayName = 'ConnectorName'

request_body.fullyQualifiedDomainName = 'CONNECTOR-MACHINE'

request_body.operatingSystem = 'Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555'

request_body.appVersion = '0.19.7338.23496'

location = PrinterLocation()
location.latitude = 1.1

location.longitude = 2.2

location.altitude_in_meters = 3


request_body.location = location



result = await client.print.connectors_by_id('printConnector-id').patch(request_body = request_body)


```