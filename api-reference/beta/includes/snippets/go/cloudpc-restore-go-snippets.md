---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphdevicemanagement "github.com/microsoftgraph/msgraph-beta-sdk-go/devicemanagement"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphdevicemanagement.NewRestorePostRequestBody()
cloudPcSnapshotId := "A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8"
requestBody.SetCloudPcSnapshotId(&cloudPcSnapshotId) 

graphClient.DeviceManagement().VirtualEndpoint().CloudPCs().ByCloudPCId("cloudPC-id").Restore().Post(context.Background(), requestBody, nil)


```