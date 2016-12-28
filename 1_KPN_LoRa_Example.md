IoT Academy 
Examples of Post Messages from Thingpark and KPN Developer Portal

Examples captured with the online tool www.hookbin.com

### KPN Developer Portal Example
Below example was generated with **SHA-Key 3b35d8e6-a146-44b1-8430-46e8bfa250d4**

**Headers**
```
Accept:application/json
Connection:close
Content-Length:546
Content-Type:application/json; charset=UTF-8
Host:hookb.in
User-Agent:Jakarta Commo
```

**Query-Parameters**
```
LrnDevEui:0059AC0000181EB6
LrnFPort:1
LrnInfos:null
AS_ID:IoTAcademy.developer
Time:2016-09-09T11:17:17.352Z
Token:27515a5c9be818a4512a233d5df0624d470d5408939fc4cba0a650961b4cc247
```

**Body**
```json
{
    "DevEUI_uplink": {
        "Time": "2016-12-21T22:15:22.135+01:00",
        "DevEUI": "0059AC0000181398",
        "FPort": "1",
        "FCntUp": "15",
        "ADRbit": "1",
        "MType": "4",
        "FCntDn": "20",
        "payload_hex": "12",
        "mic_hex": "b4998693",
        "Lrcid": "0059AC01",
        "LrrRSSI": "-104.000000",
        "LrrSNR": "-14.000000",
        "SpFact": "12",
        "SubBand": "G1",
        "Channel": "LC2",
        "DevLrrCnt": "3",
        "Lrrid": "FF0103E7",
        "Late": "0",
        "LrrLAT": "52.173420",
        "LrrLON": "5.376729",
        "Lrrs": {
            "Lrr": [
                {
                    "Lrrid": "FF0103E7",
                    "Chain": "0",
                    "LrrRSSI": "-104.000000",
                    "LrrSNR": "-14.000000",
                    "LrrESP": "-118.169540"
                },
                {
                    "Lrrid": "FF01030F",
                    "Chain": "0",
                    "LrrRSSI": "-112.000000",
                    "LrrSNR": "-5.000000",
                    "LrrESP": "-118.193314"
                },
                {
                    "Lrrid": "080E02B1",
                    "Chain": "0",
                    "LrrRSSI": "-115.000000",
                    "LrrSNR": "-13.250000",
                    "LrrESP": "-128.450775"
                }
            ]
        },
        "CustomerID": "100006356",
        "CustomerData": {
            "alr": {
                "pro": "SMTC/LoRaMote",
                "ver": "1"
            }
        },
        "ModelCfg": "0",
        "DevAddr": "14204399"
    }
}

```

### KPN ThingPark Example
Below example was created with  **SHA-Key (LRC-AS key) “00112233445566778899aabbccddeeff”**.

_To avoid confusion, in the examples the Query Parameter “Time” has been adjusted to also include a “+”, since hookbin did not display this correctly. When checking the token the + must be included in the SHA generator for the timestamp for below examples._
**Headers**
```
Accept: */* 
Connection: close 
Content-Length: 905 
Content-Type: application/json 
Host: hookb.in 
User-Agent: ACTILITY-LRCLRN-DEVICE-AGENT/1.0
```

**Query-Parameters**
```
LrnDevEui:0059AC000010020D 
LrnFPort:2 
LrnInfos:TWA_100006246.167.AS-1-1361149 
AS_ID:hookbin 
Time:2016-07-05T08:58:26.911+02:00 
Token:18f44bb294f9dd33b5168eeb92a0c7f9fa807914097dc9bb2ed5a789a65fad33
```

**Body**
```json
{ "DevEUI_uplink": { 
	"Time": "2016-07-05T08:58:26.654+02:00", 
	"DevEUI": "0059AC000010020D", 
	"FPort": "2", 
	"FCntUp": "3", 
	"ADRbit": "1", 
	"MType": "4", 
	"FCntDn": "3", 
	"payload_hex": "00277c0878fd9b2e000000000000ffff", 
	"mic_hex": "5f95a77a", 
	"Lrcid": "0059AC01", 
	"LrrRSSI": "-100.000000", 
	"LrrSNR": "5.750000", 
	"SpFact": "12", 
	"SubBand": "G0", 
	"Channel": "LC7", 
	"DevLrrCnt": "4", 
	"Lrrid": "080603DB", 
	"LrrLAT": "52.069241", 
	"LrrLON": "4.349416", 
	"Lrrs": { 
		"Lrr": [ { 
			"Lrrid": "080603DB", 
			"Chain": "0", 
			"LrrRSSI": "-100.000000", 
			"LrrSNR": "5.750000", 
			"LrrESP": "-101.024590" 
			}, 	
			{"Lrrid": "080E00C8", 
			"Chain": "0", 
			"LrrRSSI": "-118.000000", 
			"LrrSNR": "-4.000000", 
			"LrrESP": "-123.455406" 
			}, 
			{ "Lrrid": "080602C9", 
			"Chain": "0", 
			"LrrRSSI": "-119.000000", 
			"LrrSNR": "-9.500000", 
			"LrrESP": "-128.961838" } 
			] 
		}, 
	"CustomerID": "100006246", 
	"CustomerData": { "alr": { "pro": "SMTC/LoRaMote", "ver": "1" } }, 
	"ModelCfg": "0", 
	"AppSKey": "34216a533ceb98b5c811a9acf72e6822"
	} 
}
```
