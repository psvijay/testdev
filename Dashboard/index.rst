
Device Status Dashboard
=======================

Based on Trip id, you can get more detailed information of a single trip. This api is coming soon.

Get complete status of the device. 

Request
+++++++

.. code-block:: json

      POST http://dev.amberconnect.com/AmberConnectApp/public/v2.4/openapi/customersupportdashboard
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
   "Items":{
      "Latitude":"11.02124",
      "Longitude":"77.01998",
      "Address":"periyar nagar, Coimbatore",
      "ParkingFlag":"Y",
      "DateTime":"2017-05-17 12:51:48",
      "IMEI":"0358899054022275",
      "PhoneNumber":"123456",
      "LastTripDetails":{
         "success":"Y",
         "Trips":[
            {
               "Id":"LJVPI8MYN3GA20170407054524",
               "TripStartPoint":"Avinashi Road, Coimbatore, TN",
               "TripEndPoint":"Gman",
               "StartTime":"2017-04-07 05:45:25",
               "EndTime":"2017-04-07 06:31:48",
               "Distance":"16.1",
               "TopSpeed":"60",
               "Duration":"0.77",
               "Idle":"0.29",
               "Polyline":"achbAqh_uMtaB`zI]iA[cBSuB]gEo@oGMeBg@q@iCZqCPi@CMUMwHCUFaAbCwBpDoCvDkCzDwCxBmBzCuBzCiBhCqAj@c@fAe@^iBKyAWkBm@kCHeBn@Ih@CbBShAEn@?bBMHSWmB[kEm@eHc@iEaA}FuAuEo@}AkAgCeBaDuAqC{AgCsB{DcCoDcIyJ}BgDwAoCyABBH`AKeAaC}@gBiGkNqCuFaAyAQKmFsGuCyDiEaE{FqD}MqHuAq@c@c@}CkFwAeEeCgK]{DU{F_@mGeBqFuAqDy@qCYoC[uD_@_Dm@_DUsBK_ASoD}A_Oo@aJQuD]}Mo@uLXg@bCKxC?jCJhCSzBw@fDk@|Bk@Ec@gA{F",
               "LatLong":{
                  "StartPointLat":"11.024013333333",
                  "StartPointLong":"77.006337777778",
                  "EndPointLat":"11.02111",
                  "EndPointLong":"77.019937777778",
                  "MapsImage":"http:\/\/maps.googleapis.com\/maps\/api\/staticmap?size=300x300\u0026path=weight:7%7Ccolor:0x003366%7Cenc:achbAqh_uMtaB`zI]iA[cBSuB]gEo@oGMeBg@q@iCZqCPi@CMUMwHCUFaAbCwBpDoCvDkCzDwCxBmBzCuBzCiBhCqAj@c@fAe@^iBKyAWkBm@kCHeBn@Ih@CbBShAEn@?bBMHSWmB[kEm@eHc@iEaA}FuAuEo@}AkAgCeBaDuAqC{AgCsB{DcCoDcIyJ}BgDwAoCyABBH`AKeAaC}@gBiGkNqCuFaAyAQKmFsGuCyDiEaE{FqD}MqHuAq@c@c@}CkFwAeEeCgK]{DU{F_@mGeBqFuAqDy@qCYoC[uD_@_Dm@_DUsBK_ASoD}A_Oo@aJQuD]}Mo@uLXg@bCKxC?jCJhCSzBw@fDk@|Bk@Ec@gA{F\u0026markers=size:mid:http:\/\/goo.gl\/4YM8wr|11.024013333333,77.006337777778\u0026markers=size:mid:http:\/\/goo.gl\/VHRSbR|11.02111,77.019937777778"
               }
            }
         ]
      },
      "UserToken":"YA9IKHJ5MX",
      "Name":"Vijay",
      "GSMSignal":"3",
      "DeviceStatus":"Y",
      "AppStatus":"Y",
      "UserMappedStatus":"1",
      "DeviceType":"WGPS",
      "SubType":"TR06",
      "SimNumber":"",
      "SimActivateFlag":"N",
      "AmberModel":"AMB363",
      "FleetId":"651187",
      "Email":"vijay@amberconnect.com",
      "SubscriptionStartTime":"2017-02-02 06:18:54",
      "SubscriptionEndTime":"2033-01-05 09:43:08",
      "ShieldSubscriptionStartTime":"2017-01-05 09:43:08",
      "ShieldSubscriptionEndTime":"2034-01-05 09:43:08",
      "Voltage":"5",
      "TeleCutStatus":"ON",
      "TotalVoltage":"6",
      "LastAlerts":[
         {
            "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
            "HighlightText":[
               {
                  "Text":"tow alert"
               }
            ],
            "NotificationType":"MOVINGALERT",
            "DateCreated":"2017-08-10 06:55:04"
         },
         {
            "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
            "HighlightText":[
               {
                  "Text":"tow alert"
               }
            ],
            "NotificationType":"MOVINGALERT",
            "DateCreated":"2017-08-10 06:23:42"
         },
         {
            "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
            "HighlightText":[
               {
                  "Text":"tow alert"
               }
            ],
            "NotificationType":"MOVINGALERT",
            "DateCreated":"2017-08-04 07:10:05"
         },
         {
            "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
            "HighlightText":[
               {
                  "Text":"tow alert"
               }
            ],
            "NotificationType":"MOVINGALERT",
            "DateCreated":"2017-08-04 07:08:02"
         },
         {
            "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
            "HighlightText":[
               {
                  "Text":"tow alert"
               }
            ],
            "NotificationType":"MOVINGALERT",
            "DateCreated":"2017-08-01 09:25:36"
         },
         {
            "Message":"Alert! Wired India Stolen Vehicle Recovery request Closed",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
            "HighlightText":[
               {
                  "Text":"Stolen Vehicle Recovery"
               }
            ],
            "NotificationType":"RECOVERYCLOSED",
            "DateCreated":"2017-07-21 13:44:05"
         },
         {
            "Message":"Urgent! Wired India\u0027s device has been unplugged near Access Road, Coimbatore, Please check the device\u2019s connection",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/plug@2x.png",
            "HighlightText":[
               {
                  "Text":"unplugged"
               }
            ],
            "NotificationType":"POWERCUT",
            "DateCreated":"2017-07-21 13:41:07"
         },
         {
            "Message":"Alert! Wired India Stolen Vehicle Recovery request Closed",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
            "HighlightText":[
               {
                  "Text":"Stolen Vehicle Recovery"
               }
            ],
            "NotificationType":"RECOVERYCLOSED",
            "DateCreated":"2017-07-21 13:40:30"
         },
         {
            "Message":"Alert! Wired India Stolen Vehicle Recovery request Closed",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
            "HighlightText":[
               {
                  "Text":"Stolen Vehicle Recovery"
               }
            ],
            "NotificationType":"RECOVERYCLOSED",
            "DateCreated":"2017-07-21 12:31:30"
         },
         {
            "Message":"Alert! Wired India Stolen Vehicle Recovery request Closed",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
            "HighlightText":[
               {
                  "Text":"Stolen Vehicle Recovery"
               }
            ],
            "NotificationType":"RECOVERYCLOSED",
            "DateCreated":"2017-07-21 12:30:04"
         },
         {
            "Message":"Alert! Wired India Stolen Vehicle Recovery request Closed",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
            "HighlightText":[
               {
                  "Text":"Stolen Vehicle Recovery"
               }
            ],
            "NotificationType":"RECOVERYCLOSED",
            "DateCreated":"2017-07-21 12:29:59"
         },
         {
            "Message":"Urgent! Wired India\u0027s device battery is low. Please charge your Amber Connect device.",
            "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/engine_battery.png",
            "HighlightText":[
               {
                  "Text":"battery is low"
               }
            ],
            "NotificationType":"LOWBATTERY",
            "DateCreated":"2017-07-19 07:41:01"
         }
      ],
      "NightMode":[
         {
            "NightMode":"OFF",
            "NightModeStartTime":"05:10:07",
            "NightModeEndTime":"05:10:07",
            "NightModeServerStartTime":"2017-08-10 05:10:07",
            "NightModeServerEndTime":"2034-01-05 09:43:08",
            "ModeType":"SentryModeType",
            "NightModeUpdatedTime":"2017-08-10 05:10:09",
            "Hours":"",
            "SentryModeType":"OFF",
            "LockModeType":"OFF",
            "NightModeType":"OFF"
         }
      ],
      "DeviceName":"Wired India",
      "BufferedTripsCount":"0",
      "AmberAuthToken":"LJVPI8MYN3GA",
      "TripCount":"1421",
      "AlertsCount":"8018",
      "HeartBeatPacketCount":"8",
      "LastHeartBeatTime":"2017-05-17 12:48:31"
   },
   "ServerCurrentTime":"2017-09-05 17:48:35",
   "ServerTimezone":"UTC",
   "ServerTz":"UTC"
 }
	  
