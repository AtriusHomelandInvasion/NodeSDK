NodeSDK
=======

Playfab SDK for node.js applications

This SDK includes all PlayFab APIs (Client, Server, Admin) in a single javascript file suitable for using in node.js.

Usage:
```
var playfab = require('./playfab.js')

playfab.settings.title_id = "F00";
playfab.settings.developer_secret_key = "XXX";

playfab.server.GetTitleData({Keys : ["Sample"]}, function(error, result)
{
	if(error)
	{
		console.log("Got an error: ",error);
		return;
	}

	console.log("Reply: ",result);
});

```
