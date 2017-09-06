Live Tracking
=============
Track any vehicle Live. Api end point: "getlivetracking" - This api end point returns the live information about the  vehicle. 

Request
+++++++

.. code-block:: json

      POST http://dev.amberconnect.com/AmberConnectApp/public/v2.4/openapi/getlivetracking
      Accept: application/json

* `DeviceOffset` - Mandatory, Default=0
* `AmberAuthToken` - Mandatory, Amber device's unique QR code.
* `APIKey` - Mandatory
* `Currency` - Optional parameter. Default to User's Currency.
* `DistanceUnit` - Optional parameter. Default to User's measurement unit.



Response
++++++++

.. code-block:: json

      HTTP/1.1 200 OK
      Content-Type: application/json
	  
	  {
   "success":"Y",
   "Details":{
      "Latitude":"11.02124",
      "Longitude":"77.01998",
      "IgnitionStatus":"1",
      "DrivingDirection":"679",
      "GSMSignal":"3",
      "LiveDistance":"",
      "LiveTripStartTime":"2017-05-17 12:51:25",
      "LiveTripEndTime":"2017-05-17 12:51:48",
      "LiveTripId":"LJVPI8MYN3GA20170517125016",
      "OdometerReading":"326792",
      "FuelTankCapacity":"999.0",
      "CurrentFuelLevel":"999",
      "LiveRunTime":"",
      "LiveFuel":"",
      "ParkIdleTime":"",
      "LiveHA":"0",
      "LiveSB":"0",
      "Mileage":"12",
      "AmberModel":"AMB363",
      "DeviceSubType":"TR06",
      "LiveSpeeding":"0",
      "LiveIdleTime":"0",
      "ParkingFlag":"N",
      "DateTime":"2017-05-17 12:51:48",
      "Speed":"10",
      "IMEI":"0358899054022275",
      "Voltage":"5",
      "TotalVoltage":"6",
      "DeviceCategory":"CAR",
      "LastHeartBeatTime":"",
      "DeviceType":"Wired GPS"
   },
   "ServerCurrentTime":"2017-09-05 17:33:35",
   "ServerTimezone":"UTC",
   "ServerTz":"UTC"
 }