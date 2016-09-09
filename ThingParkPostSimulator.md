IoT Academy - ThingPark Simulator
Created by Michiel Jol 

Below you will find a curl command to post a standard example,
from KPN /Actility ThingPark to your own server (J-SON format).

The post is directed to **https://example.yourserver.com/postlistener**. 
Please adjust the destination to your own specifics

We recommend using Postman (Chrome App) to execute the cURL command:
Use the Import function and copy paste the lines below to easily adjust 
and visualize posts.

You can set up your Server to receive post message. To check
the implemenation of your SHA256 token generation you can use the
**AS-Key : “00112233445566778899aabbccddeeff”** and should be able to
generate the received token. 
_NOTE: Some POST receivers exclude the "+" included in the timestamp
but the "+" must be given to SHA256 to get a correct token!_

Post was initialy caught by the free HTTPS POST catcher www.hookbin.com
Example created by Postman (Chrome App). 

--- COPY LINES BELOW ----
`curl -X POST -H "Accept: */*" -H "Content-Type: application/json" -H "Cache-Control: no-cache" -d '{ "DevEUI_uplink": { "Time": "2016-07-05T08:58:26.654+02:00", "DevEUI": "0059AC000010020D", "FPort": "2", "FCntUp": "3", "ADRbit": "1", "MType": "4", "FCntDn": "3", "payload_hex": "00277c0878fd9b2e000000000000ffff", "mic_hex": "5f95a77a", "Lrcid": "0059AC01", "LrrRSSI": "-100.000000", "LrrSNR": "5.750000", "SpFact": "12", "SubBand": "G0", "Channel": "LC7", "DevLrrCnt": "4", "Lrrid": "080603DB", "LrrLAT": "52.069241", "LrrLON": "4.349416", "Lrrs": { "Lrr": [ { "Lrrid": "080603DB", "Chain": "0", "LrrRSSI": "-100.000000", "LrrSNR": "5.750000", "LrrESP": "-101.024590" }, {"Lrrid": "080E00C8", "Chain": "0", "LrrRSSI": "-118.000000", "LrrSNR": "-4.000000", "LrrESP": "-123.455406" }, { "Lrrid": "080602C9", "Chain": "0", "LrrRSSI": "-119.000000", "LrrSNR": "-9.500000", "LrrESP": "-128.961838" } ] }, "CustomerID": "100006246", "CustomerData": { "alr": { "pro": "SMTC/LoRaMote", "ver": "1" } }, "ModelCfg": "0", "AppSKey": "34216a533ceb98b5c811a9acf72e6822" } }' "https://example.yourserver.com/postlistener?LrnDevEui=0059AC000010020D&LrnFPort=2&LrnInfos=TWA_100006246.167.AS-1-1361149&AS_ID=hookbin&Time=2016-07-05T08:58:26.911+02:00&Token=18f44bb294f9dd33b5168eeb92a0c7f9fa807914097dc9bb2ed5a789a65fad33"`
