---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new LogTeleconferenceDeviceQualityPostRequestBody
{
	Quality = new TeleconferenceDeviceQuality
	{
		OdataType = "#microsoft.graph.teleconferenceDeviceQuality",
		CallChainId = "0622673d-9f69-49b3-9d4f-5ec64f42ecce",
		ParticipantId = "ea078406-b5d4-4d3c-b85e-90103dcec7f6",
		MediaLegId = "bd9ee398-4b9d-42c7-8b8d-4e8efad9435f",
		DeviceName = "TestAgent",
		DeviceDescription = "TestDescription",
		MediaQualityList = new List<TeleconferenceDeviceMediaQuality>
		{
			new TeleconferenceDeviceMediaQuality
			{
				AdditionalData = new Dictionary<string, object>
				{
					{
						"@odata.type" , "#microsoft.graph.teleconferenceDeviceAudioQuality"
					},
					{
						"channelIndex" , 1
					},
					{
						"mediaDuration" , "PT20M"
					},
					{
						"networkLinkSpeedInBytes" , 13000
					},
					{
						"localIPAddress" , "127.0.0.1"
					},
					{
						"localPort" , 6300
					},
					{
						"remoteIPAddress" , "102.1.1.101"
					},
					{
						"remotePort" , 6301
					},
					{
						"inboundPackets" , 5500
					},
					{
						"outboundPackets" , 5400
					},
					{
						"averageInboundPacketLossRateInPercentage" , 0.01
					},
					{
						"averageOutboundPacketLossRateInPercentage" , 0.02
					},
					{
						"maximumInboundPacketLossRateInPercentage" , 0.05
					},
					{
						"maximumOutboundPacketLossRateInPercentage" , 0.06
					},
					{
						"averageInboundRoundTripDelay" , "PT0.03S"
					},
					{
						"averageOutboundRoundTripDelay" , "PT0.04S"
					},
					{
						"maximumInboundRoundTripDelay" , "PT0.13S"
					},
					{
						"maximumOutboundRoundTripDelay" , "PT0.14S"
					},
					{
						"averageInboundJitter" , "PT0.01S"
					},
					{
						"averageOutboundJitter" , "PT0.015S"
					},
					{
						"maximumInboundJitter" , "PT0.023S"
					},
					{
						"maximumOutboundJitter" , "PT0.024S"
					},
				},
			},
			new TeleconferenceDeviceMediaQuality
			{
				AdditionalData = new Dictionary<string, object>
				{
					{
						"@odata.type" , "#microsoft.graph.teleconferenceDeviceVideoQuality"
					},
					{
						"channelIndex" , 1
					},
					{
						"mediaDuration" , "PT20M"
					},
					{
						"networkLinkSpeedInBytes" , 13000
					},
					{
						"localIPAddress" , "127.0.0.1"
					},
					{
						"localPort" , 6300
					},
					{
						"remoteIPAddress" , "102.1.1.101"
					},
					{
						"remotePort" , 6301
					},
					{
						"inboundPackets" , 5500
					},
					{
						"outboundPackets" , 5400
					},
					{
						"averageInboundPacketLossRateInPercentage" , 0.01
					},
					{
						"averageOutboundPacketLossRateInPercentage" , 0.02
					},
					{
						"maximumInboundPacketLossRateInPercentage" , 0.05
					},
					{
						"maximumOutboundPacketLossRateInPercentage" , 0.06
					},
					{
						"averageInboundRoundTripDelay" , "PT0.03S"
					},
					{
						"averageOutboundRoundTripDelay" , "PT0.04S"
					},
					{
						"maximumInboundRoundTripDelay" , "PT0.13S"
					},
					{
						"maximumOutboundRoundTripDelay" , "PT0.14S"
					},
					{
						"averageInboundJitter" , "PT0.01S"
					},
					{
						"averageOutboundJitter" , "PT0.015S"
					},
					{
						"maximumInboundJitter" , "PT0.023S"
					},
					{
						"maximumOutboundJitter" , "PT0.024S"
					},
				},
			},
			new TeleconferenceDeviceMediaQuality
			{
				AdditionalData = new Dictionary<string, object>
				{
					{
						"@odata.type" , "#microsoft.graph.teleconferenceDeviceScreenSharingQuality"
					},
					{
						"channelIndex" , 1
					},
					{
						"mediaDuration" , "PT20M"
					},
					{
						"networkLinkSpeedInBytes" , 13000
					},
					{
						"localIPAddress" , "127.0.0.1"
					},
					{
						"localPort" , 6300
					},
					{
						"remoteIPAddress" , "102.1.1.101"
					},
					{
						"remotePort" , 6301
					},
					{
						"inboundPackets" , 5500
					},
					{
						"outboundPackets" , 5400
					},
					{
						"averageInboundPacketLossRateInPercentage" , 0.01
					},
					{
						"averageOutboundPacketLossRateInPercentage" , 0.02
					},
					{
						"maximumInboundPacketLossRateInPercentage" , 0.05
					},
					{
						"maximumOutboundPacketLossRateInPercentage" , 0.06
					},
					{
						"averageInboundRoundTripDelay" , "PT0.03S"
					},
					{
						"averageOutboundRoundTripDelay" , "PT0.04S"
					},
					{
						"maximumInboundRoundTripDelay" , "PT0.13S"
					},
					{
						"maximumOutboundRoundTripDelay" , "PT0.14S"
					},
					{
						"averageInboundJitter" , "PT0.01S"
					},
					{
						"averageOutboundJitter" , "PT0.015S"
					},
					{
						"maximumInboundJitter" , "PT0.023S"
					},
					{
						"maximumOutboundJitter" , "PT0.024S"
					},
				},
			},
		},
	},
};
await graphClient.Communications.Calls.LogTeleconferenceDeviceQuality.PostAsync(requestBody);


```