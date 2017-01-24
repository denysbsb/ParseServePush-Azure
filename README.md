# ParseServePush-Azure
Parse serve push notification in Azure Cloud

- First create account azure 
- Install server nodejs copy credentials
- Install mongodb copy credentials
- In portal azure Your Application > DEVELOPMENT TOOLS > App Service Editor
- Deploy code in you path wwwroot
- Configure config.js

`{ server: 
   { appId: 'YourAPI',
     masterKey: 'Youmasterkey',
     databaseURI: 'mongodb://YOUMONGO/parse?ssl=true',
     serverURL: 'Youurl',
     cloud: 'D:\\home\\site\\wwwroot/cloud/main.js',
     logFolder: 'D:\\home\\site\\wwwroot/logs',
     filesAdapter: [Function],
     push: { adapter: [Function] },
     allowClientClassCreation: false,
     enableAnonymousUsers: false },
  dashboard: { apps: [ [Object] ], users: [ [Object] ] },
  push: 
   { HubName: 'YOUname-hub',
     ConnectionString: 'Endpoint=sb://YOUHUB' },
  storage: 
   { name: 'Youstorage',
     container: 'parse',
     accessKey: 'YouaccesskeyStorage',
     directAccess: true } }`
     
- Open of App Service Editor > Console write 'npm intall'
- Restart service

To use API parse use `https://{MY_URL}/parse/classes/{myclass}` GET/POST/PUT/DELETE 
