---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphusers "github.com/microsoftgraph/msgraph-beta-sdk-go/users"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphusers.NewSetStatusMessagePostRequestBody()
statusMessage := graphmodels.NewPresenceStatusMessage()
message := graphmodels.NewItemBody()
content := "Hey I'm currently in a meeting."
message.SetContent(&content) 
contentType := graphmodels.TEXT_BODYTYPE 
message.SetContentType(&contentType) 
statusMessage.SetMessage(message)
expiryDateTime := graphmodels.NewDateTimeTimeZone()
dateTime := "2022-10-18T17:05:33.2079781"
expiryDateTime.SetDateTime(&dateTime) 
timeZone := "Pacific Standard Time"
expiryDateTime.SetTimeZone(&timeZone) 
statusMessage.SetExpiryDateTime(expiryDateTime)
requestBody.SetStatusMessage(statusMessage)

graphClient.Users().ByUserId("user-id").Presence().SetStatusMessage().Post(context.Background(), requestBody, nil)


```