---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrintConnector()
request_body.setDisplayName('ConnectorName')

request_body.setFullyQualifiedDomainName('CONNECTOR-MACHINE')

request_body.setOperatingSystem('Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555')

request_body.setAppVersion('0.19.7338.23496')

location = PrinterLocation()
location.setLatitude(1.1)

location.setLongitude(2.2)

location.setAltitudeInMeters(3)


request_body.setLocation($location)


result = await client.print.connectors._by_id('printConnector-id').patch(request_body)


```