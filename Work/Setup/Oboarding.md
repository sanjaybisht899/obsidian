


Onboarding

* APPLICATION_SECRET=E4MKTTmJ7y6L2d8D7cZk3Cp3wqR8U591CK6tF1doOhc= node app/tasks/import_client.js --client collection
* node app/tasks/import_client.js --client collection
* node import_new.js --client='collection' all --init

After Onboarding is done  Copy Hash

`"salt" : "fwlf5LPoeUFw206pzcKJnA==",` 
`"hashed_password" : "r1B4T4Nqc5bLMtl3k4dWSrjX6OATp654A/XYBsFDHYvXXHOstVZfWuS7VA7Y2Q/PH7lZc4HhQqKM1VcFsaNfbA==",`


After that

* curl -X POST "[http://localhost:8080/sso/config/client/sync](http://localhost:8080/sso/config/client/sync)" -H 'cache-control: no-cache' -d 'client=agency&sso_login=true' 
* curl -X PUT "[http://localhost:8082/status?user=divya](http://localhost:8082/status?user=divya)" -H 'content-type: application/json' -d '{"path":"clients.agency","key":"active","value":"true"}'
* curl -v "[http://localhost:8082/sync](http://localhost:8082/sync)"

