IoT Academy - KPN Developer Portal Simulator
Created by Michiel Jol 

Below you will find a curl command to post a standard example,
from the KPN LoRa Developer Portal to your own server.

The post is directed to **https://example.yourserver.com/postlistener**. 
Please adjust the destination to your own specifics

We recommend using Postman (Chrome App) to execute the cURL command:
Use the Import function and copy paste the lines below to easily adjust 
and visualize posts.

You can set up your Server to receive post message. To check
the implemenation of your SHA256 token generation you can use the
**AS-Key : “3b35d8e6-a146-44b1-8430-46e8bfa250d4”** and should be able to
generate the received token. 

Post was initialy caught by the free HTTPS POST catcher www.hookbin.com.
Example created by Postman (Chrome App). 

```
curl -X POST -H "Accept: application/json" -H "Connection: close" -H "Content-Length: 546" -H "Content-Type: application/json; charset=UTF-8" -H "Host: hookb.in" -H "User-Agent: Jakarta Commons-HttpClient/3.1" -H "Cache-Control: no-cache" -d '{
    "LrrSNR": "9.000000",
    "Lrrid": "FF010345",
    "SpFact": 7,
    "SubBand": "G1",
    "CustomerData": "{\"alr\":{\"pro\":\"SMTC/LoRaMote\",\"ver\":\"1\"}}",
    "FPort": 1,
    "Channel": "LC3",
    "FCntUp": 0,
    "Time": 1473419836813,
    "DevEUI": "0059AC0000181EB6",
    "payload_hex": "effe",
    "CustomerID": 100006356,
    "LrrRSSI": "-100.000000",
    "ADRbit": 1,
    "ModelCfg": 0,
    "mic_hex": "e87053fe",
    "LrrLON": "4.329981",
    "LrrLAT": "52.056404",
    "FCntDn": 1,
    "Lrcid": "0059AC01",
    "DevLrrCnt": 2
}' "https://example.yourserver.com/postlistener.?LrnDevEui=0059AC0000181EB6&LrnFPort=1&LrnInfos=null&AS_ID=IoTAcademy.developer&Time=2016-09-09T11:17:17.352Z&Token=27515a5c9be818a4512a233d5df0624d470d5408939fc4cba0a650961b4cc247"
```
