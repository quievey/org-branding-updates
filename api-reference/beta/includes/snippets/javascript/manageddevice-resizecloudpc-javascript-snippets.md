---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/managedDevices/{managedDeviceId}/resizeCloudPc')
	.version('beta')
	.post();

```