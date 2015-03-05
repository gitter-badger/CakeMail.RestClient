[![Build status](https://ci.appveyor.com/api/projects/status/fd008gl72j4wyi84?svg=true)](https://ci.appveyor.com/project/Jericho/cakemailrestapi)

# CakeMailRestAPI

## About

CakeMailRestAPI is a C# client for the CakeMail service through its RESTful API.

## Features


## Contact

You can contact me on Twitter [@NorthernNomad](https://twitter.com/northernnomad).

## Nuget

CakeMailRestAPI will eventually be available as a Nuget package.

## Release Notes

+ **1.0.0**    Initial release
 
## Usage

```csharp
var apiKey = "... your api key ...";
var userName = "youremail@whatever.com";
var password = "yourpassword";

var client = new Client(apiKey);

var loginInfo = client.Login(userName, password);
var user = client.GetUser(loginInfo.UserKey, loginInfo.UserId, loginInfo.ClientId);
```
