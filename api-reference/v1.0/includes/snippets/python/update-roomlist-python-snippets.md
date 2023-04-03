---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Place();
requestBody.set@odatatype('microsoft.graph.roomList');

requestBody.setDisplayName('Building 1');

requestBody.setPhone('555-555-0100');

address = PhysicalAddress();
address.setStreet('4567 Main Street');

address.setCity('Buffalo');

address.setState('NY');

address.setPostalCode('98052');

address.setCountryOrRegion('USA');


requestBody.setAddress($address);
geoCoordinates = OutlookGeoCoordinates();
GeoCoordinates.setAltitude(null);

geoCoordinates.setLatitude(47);

geoCoordinates.setLongitude(-122);

GeoCoordinates.setAccuracy(null);

GeoCoordinates.setAltitudeAccuracy(null);


requestBody.setGeoCoordinates($geoCoordinates);


result = awaitclient.placesById('place-id').patch(requestBody);


```