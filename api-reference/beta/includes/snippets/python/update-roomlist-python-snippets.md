---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Place()
request_body.@odatatype = 'microsoft.graph.roomList'

request_body.displayName = 'Building 1'

request_body.phone = '555-555-0100'

address = PhysicalAddress()
address.street = '4567 Main Street'

address.city = 'Buffalo'

address.state = 'NY'

address.postalCode = '98052'

address.countryOrRegion = 'USA'


request_body.address = address
geoCoordinates = OutlookGeoCoordinates()
GeoCoordinates.altitude=null

geoCoordinates.latitude = 47

geoCoordinates.longitude = -122

GeoCoordinates.accuracy=null

GeoCoordinates.altitudeAccuracy=null


request_body.geoCoordinates = geoCoordinates


request_configuration = PlaceRequestBuilderPatchRequestConfiguration(
)


result = await client.places_by_id('place-id').patch(request_body = request_body)


```