# Kuna camera web API


This is my attempt to document the KUNA api in the hopes that I can do a little more automation.   

First the basics


```
restScheme=https
server=server.kunasystems.com
port=443
apiVersion=/api/v1/
authentication=account/auth/
getCameras=user/cameras/
getCamera=cameras/$/
getCameraInfo=cameras/$/info
getRecordings=recordings/
getTimezones=timezones/
getUser=user/
getUserNews=user/news/
getToken=cameras/
registerGcm=push/gcm/
unregisterGcm=push/gcm/$/
createUser=users/
forgotPassword=account/password/reset/
```

If you visit https://server.kunasystems.com/api/v1/user/cameras/  when logged in you get interesting json.  Likewise for things like camera details (https://server.kunasystems.com/api/v1/cameras/MY_CAMERA_ID/) and so on (you can GET most of the things specified and intersting JSON is returned

Sadly there is no obvious way to 'set' parameters -- a try to POST or PUT with a JSON paypload of values returns a 'page not found'

so there you have it.

I'm tossing this out there both as a set of notes as I plow through trying to sort out how to make it work but also hoping someone can contribute.  

Really I have pretty modest goals -- if I could remotely enable/disable alerts that is most of what I want!


