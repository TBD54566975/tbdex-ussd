# tbdex-ussd

An experiment to show how USSD can work with web5. 

USSD (https://www.techtarget.com/searchnetworking/definition/USSD) is often used for access to payment services from non 
smart phones in various parts of the world and is an extremely lightweight protocol. 

This is based on the excellent article https://moses-odhiambo-dev.medium.com/creating-a-ussd-application-with-nodejs-and-redis-part-1-347cf1cd7a61 by Moses Odhiambo.

# Runnning

```
npm install
npm run serve
```

Then in another window: 

```
  cloudflared tunnel --url http://localhost:3030
```

This will give you a publicly accessible USSD endpoint. To try it out, sign up for a free account at https://africastalking.com/ - and then go to the sandbox and register the USSD channel. 

Fun!

![dial](https://github.com/TBD54566975/tbdex-ussd/assets/14976/1067c45a-08fb-46fc-b0ac-d88748e34f45)
![phone](https://github.com/TBD54566975/tbdex-ussd/assets/14976/1a290223-9b66-4b0c-90f0-c0c2d11c9981)

Be sure to take a look at the guide: https://moses-odhiambo-dev.medium.com/creating-a-ussd-application-with-nodejs-and-redis-part-1-347cf1cd7a61 
