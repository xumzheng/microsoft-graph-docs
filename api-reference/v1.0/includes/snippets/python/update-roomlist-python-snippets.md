---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Place();
request_body.set@odatatype('microsoft.graph.roomList');

request_body.setDisplayName('Building 1');

request_body.setPhone('555-555-0100');

address = PhysicalAddress();
address.setStreet('4567 Main Street');

address.setCity('Buffalo');

address.setState('NY');

address.setPostalCode('98052');

address.setCountryOrRegion('USA');


request_body.setAddress($address);
geoCoordinates = OutlookGeoCoordinates();
GeoCoordinates.setAltitude(null);

geoCoordinates.setLatitude(47);

geoCoordinates.setLongitude(-122);

GeoCoordinates.setAccuracy(null);

GeoCoordinates.setAltitudeAccuracy(null);


request_body.setGeoCoordinates($geoCoordinates);


result = await client.placesById('place-id').patch(request_body);


```