Here you can find an example of a DevEUI_location message originating from Thingpark for a device that is configured for localisation. This message will be send as soon as the LRC has calculated the location.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<DevEUI_location
    xmlns="http://uri.actility.com/lora">
    <DevEUI>0018B2000067BCDE</DevEUI>
    <DevAddr>0467BCDE</DevAddr>
    <Lrcid>0059AC01</Lrcid>
    <Time>2016-10-11T15:08:52.0+02:00</Time>
    <DevLocTime>2016-10-11T15:08:52.0+02:00</DevLocTime>
    <DevLAT>52.068363</DevLAT>
    <DevLON>5.192625</DevLON>
    <DevAlt>33.500000</DevAlt>
    <DevAcc>0.000000</DevAcc>
    <DevLocRadius>0.000000</DevLocRadius>
    <DevAltRadius>0.000000</DevAltRadius>
    <CustomerID>100006241</CustomerID>
</DevEUI_location>
```
