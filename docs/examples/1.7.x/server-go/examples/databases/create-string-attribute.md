package main

import (
    "fmt"
    "github.com/appwrite/sdk-for-go/client"
    "github.com/appwrite/sdk-for-go/databases"
)

func main() {
    client := client.NewClient()

    client.SetEndpoint("https://<REGION>.cloud.appwrite.io/v1") // Your API Endpoint
    client.SetProject("<YOUR_PROJECT_ID>") // Your project ID
    client.SetKey("<YOUR_API_KEY>") // Your secret API key

    service := databases.NewDatabases(client)
    response, error := service.CreateStringAttribute(
        "<DATABASE_ID>",
        "<COLLECTION_ID>",
        "",
        1,
        false,
        databases.WithCreateStringAttributeDefault("<DEFAULT>"),
        databases.WithCreateStringAttributeArray(false),
        databases.WithCreateStringAttributeEncrypt(false),
    )

    if error != nil {
        panic(error)
    }

    fmt.Println(response)
}
