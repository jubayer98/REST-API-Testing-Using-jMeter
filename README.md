# REST-API-Testing-Using-jMeter
REST API: REST or RESTful API design (Representational State Transfer) is designed to take advantage of existing protocols. While REST can be used over nearly any protocol, it usually takes advantage of HTTP when used for Web APIs. This means that developers do not need to install libraries or additional software in order to take advantage of a REST API design. 

REST API:
REST or RESTful API design (Representational State Transfer) is designed to take advantage of existing
protocols. While REST can be used over nearly any protocol, it usually takes advantage of HTTP when used
for Web APIs. This means that developers do not need to install libraries or additional software in order to
take advantage of a REST API design.

Procedure:

Step 1:
Add HTTP Request Sampler for REST API

Step 2:
http://openweathermap.org/api - Testing Website
5f9929442e57f662a038a8fc0ed3db0e – My API Key
http://samples.openweathermap.org/data/2.5/weather?q=dhaka&appid=5f9929442e57f662a038a8fc0ed3db0e
samples.openweathermap.org – IP of Particular Web Services
/data/2.5/weather/ – Path Where We Have to Go
q=dhaka&appid=5f9929442e57f662a038a8fc0ed3db0e – Parameters

Step 3:
Set the value in HTTP Request Sampler and add the parameter value and run the test.
Table WAI TER Kitchen
RESTAURANT
Role of WAITER is API

Results:

Sampler Result:
Thread Name: Thread Group 1-1
Sample Start: 2017-11-18 17:38:49 BDT
Load time: 634
Connect Time: 404
Latency: 634
Size in bytes: 917
Sent bytes:193
Headers size in bytes: 446
Body size in bytes: 471
Sample Count: 1
Error Count: 0
Data type ("text"|"bin"|""): text
Response code: 200
Response message: OK
Response headers:
HTTP/1.1 200 OK
Server: openresty/1.9.7.1
Date: Sat, 18 Nov 2017 11:38:49 GMT
Content-Type: application/json; charset=utf-8
Transfer-Encoding: chunked
Connection: keep-alive
X-Frame-Options: SAMEORIGIN
X-XSS-Protection: 1; mode=block
X-Content-Type-Options: nosniff
ETag: W/"e70c27085ed41de5321252b16c9582fe"
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: ded5c51a-8492-429d-8d3c-5e8dd6d0eebe
X-Runtime: 0.001512
HTTPSampleResult fields:
ContentType: application/json; charset=utf-8
DataEncoding: utf-8
Request:
GET
http://samples.openweathermap.org/data/2.5/weather?q=dhaka&appid=5f9929442e57f662a038a
8fc0ed3db0e
GET data:
[no cookies]
Request Headers:
Connection: keep-alive
Host: samples.openweathermap.org
User-Agent: Apache-HttpClient/4.5.3 (Java/1.8.0_151)
Response Data:
{"coord":{"lon":-
0.13,"lat":51.51},"weather":[{"id":300,"main":"Drizzle","description":"light intensity
drizzle","icon":"09d"}],"base":"stations","main":{"temp":280.32,"pressure":1012,"humid
ity":81,"temp_min":279.15,"temp_max":281.15},"visibility":10000,"wind":{"speed":4.1,"d
eg":80},"clouds":{"all":90},"dt":1485789600,"sys":{"type":1,"id":5091,"message":0.0103
,"country":"GB","sunrise":1485762037,"sunset":1485794875},"id":2643743,"name":"London"
,"cod":200}
The whole procedure can be done by using REST/XML – RPC Request with more efficient way. There
variable doesn’t declare in separate way. Only a URL is enough to do with this testing. But this request
sampler are now deprecated because of BUG 60727.
