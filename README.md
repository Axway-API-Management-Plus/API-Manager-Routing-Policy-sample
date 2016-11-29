# Description
API Manager Routing policy sample 
Provided sample uses Stock Quote and Exchange Rates REST APIs for backend and the routing is done based on value specified in a custom header Backend-Service. 
Related policies and API Manager export are also provided.


## API Management Version Compatibilty
This artefact was successfully tested for the following versions:
- To be completed


## Install
- Create a Routing Policy (Could simply have one filter to route to a backend or have a branch to route to backend services based on incoming content)
  
![alt text][Screenshot1]
[Screenshot1]: https://github.com/Axway-API-Management/API-Manager-Routing-Policy-sample/blob/master/Readme/Screenshot1.png  "Screenshot1"   
  
- Add the routing policy in Policy Studio under Server Settings > API Manager > Routing Policies and deploy so it is available within API Manager UI
  
![alt text][Screenshot2]
[Screenshot2]: https://github.com/Axway-API-Management/API-Manager-Routing-Policy-sample/blob/master/Readme/Screenshot2.png  "Screenshot2"   
  
- Create a dummy Backend API (the URI could be valid or dummy) and a Front-end API based on this. Then in the Outbound tab, select the policy in the Default Method Routing dropdown
  
![alt text][Screenshot3]
[Screenshot3]: https://github.com/Axway-API-Management/API-Manager-Routing-Policy-sample/blob/master/Readme/Screenshot3.png  "Screenshot3"   
  
- Save/Publish the Front-end API and test (use HTTP header Backend-Service to pass the required backend service to be routed to)
  
  * Traffic Monitor:

![alt text][Screenshot4]
[Screenshot4]: https://github.com/Axway-API-Management/API-Manager-Routing-Policy-sample/blob/master/Readme/Screenshot4.png  "Screenshot4"   

  * Custom routing policy execution path:
  
![alt text][Screenshot5]
[Screenshot5]: https://github.com/Axway-API-Management/API-Manager-Routing-Policy-sample/blob/master/Readme/Screenshot5.png  "Screenshot5"   


As you can see, there can be Request and Response policies configured for each Front-end API (and individual method) for any validation/enrichment/transformation.


## Usage
```
To be completed
```
   

## Bug and Caveats

```
To be completed
```

## Contributing

Please read [Contributing.md] (/Contributing.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Team

![alt text][Axwaylogo] Axway Team

[Axwaylogo]: https://github.com/Axway-API-Management/Common/blob/master/img/AxwayLogoSmall.png  "Axway logo"


## License
Apache License 2.0 (refer to document [license] (https://github.com/Axway-API-Management/Executing-loopback-requests-on-a-listener/blob/master/LICENSE))

