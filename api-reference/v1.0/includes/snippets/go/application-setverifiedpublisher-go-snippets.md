---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphapplications "github.com/microsoftgraph/msgraph-sdk-go/applications"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphapplications.NewSetVerifiedPublisherPostRequestBody()
verifiedPublisherId := "1234567"
requestBody.SetVerifiedPublisherId(&verifiedPublisherId) 

graphClient.Applications().ByApplicationId("application-id").SetVerifiedPublisher().Post(context.Background(), requestBody, nil)


```