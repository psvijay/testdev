List Safety Alerts
==================


Get the safety alerts generated for vehicle. Api end point : "listalerts" returns the live information about the  vehicle. 

Request
+++++++

.. code-block:: json

      POST http://dev.amberconnect.com/AmberConnectApp/public/v2.4/openapi/listalerts
      Accept: application/json

* `DeviceOffset` - Mandatory, Default=0
* `AmberAuthToken` - Mandatory, Amber device's unique QR code.
* `APIKey` - Mandatory
* `AlertType` - Optional parameter to filter alert based on types. 
* `CustomStartDate` - Optional parameter. Filter possible by start and end date together
* `CustomEndDate` - Optional parameter. Filter possible by start and end date together
* `Currency` - Optional parameter. Default to User's Currency.
* `DistanceUnit` - Optional parameter. Default to User's measurement unit.
* `Page` - Mandatory for pagination. Starts with 1 and ends based on result set count and Limit parameter.
* `Limit` - Mandatory for pagination. Per page results limited to default/max 15 records.


Response
++++++++

.. code-block:: json

      HTTP/1.1 200 OK
      Content-Type: application/json
	  
	  {
   "success":"Y",
   "SubscriptionFlag":"Y",
   "SubscriptionLink":"http:\/\/amberconnect.com\/",
   "count":"8018",
   "start":"1",
   "end":"15",
   "CarAlerts":[
      {
         "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
         "Location":" Access Road, Coimbatore",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"tow alert"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"MOVINGALERT",
         "DateCreated":"2017-08-10 06:55:04"
      },
      {
         "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
         "Location":" Access Road, Coimbatore",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"tow alert"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"MOVINGALERT",
         "DateCreated":"2017-08-10 06:23:42"
      },
      {
         "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
         "Location":" Access Road, Coimbatore",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"tow alert"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"MOVINGALERT",
         "DateCreated":"2017-08-04 07:10:05"
      },
      {
         "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
         "Location":" Access Road, Coimbatore",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"tow alert"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"MOVINGALERT",
         "DateCreated":"2017-08-04 07:08:02"
      },
      {
         "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
         "Location":" Access Road, Coimbatore",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"tow alert"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"MOVINGALERT",
         "DateCreated":"2017-08-01 09:25:36"
      },
      {
         "Message":"Alert! Wired India Stolen Vehicle Recovery request Closed",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
         "Location":"",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"Stolen Vehicle Recovery"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"RECOVERYCLOSED",
         "DateCreated":"2017-07-21 13:44:05"
      },
      {
         "Message":"Urgent! Wired India\u0027s device has been unplugged near Access Road, Coimbatore, Please check the device\u2019s connection",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/plug@2x.png",
         "Location":" Access Road, Coimbatore, Please check the device\u2019s connection",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"unplugged"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"POWERCUT",
         "DateCreated":"2017-07-21 13:41:07"
      },
      {
         "Message":"Alert! Wired India Stolen Vehicle Recovery request Closed",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
         "Location":"",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"Stolen Vehicle Recovery"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"RECOVERYCLOSED",
         "DateCreated":"2017-07-21 13:40:30"
      },
      {
         "Message":"Alert! Wired India Stolen Vehicle Recovery request Closed",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
         "Location":"",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"Stolen Vehicle Recovery"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"RECOVERYCLOSED",
         "DateCreated":"2017-07-21 12:31:30"
      },
      {
         "Message":"Alert! Wired India Stolen Vehicle Recovery request Closed",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
         "Location":"",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"Stolen Vehicle Recovery"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"RECOVERYCLOSED",
         "DateCreated":"2017-07-21 12:30:04"
      },
      {
         "Message":"Alert! Wired India Stolen Vehicle Recovery request Closed",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
         "Location":"",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"Stolen Vehicle Recovery"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"RECOVERYCLOSED",
         "DateCreated":"2017-07-21 12:29:59"
      },
      {
         "Message":"Urgent! Wired India\u0027s device battery is low. Please charge your Amber Connect device.",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/engine_battery.png",
         "Location":"",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"battery is low"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"LOWBATTERY",
         "DateCreated":"2017-07-19 07:41:01"
      },
      {
         "Message":"Urgent! Wired India is being towed near Access Road, Coimbatore",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/vibration.png",
         "Location":" Access Road, Coimbatore",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"tow alert"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"MOVINGALERT",
         "DateCreated":"2017-07-18 10:18:24"
      },
      {
         "Message":"Urgent! Wired India\u0027s device battery is low. Please charge your Amber Connect device.",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/engine_battery.png",
         "Location":"",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"battery is low"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"LOWBATTERY",
         "DateCreated":"2017-07-17 11:40:13"
      },
      {
         "Message":"Alert! Stolen Vehicle Recovery request for Wired India initiated near periyar nagar, Coimbatore",
         "Image":"http:\/\/dev.amberconnect.com\/AmberConnectApp\/data\/images\/help_king.png",
         "Location":" periyar nagar, Coimbatore",
         "CarName":"Wired India",
         "HighlightText":[
            {
               "Text":"Stolen Vehicle Recovery"
            }
         ],
         "IdleTimeMins":"",
         "NotificationType":"RECOVERYOPEN",
         "DateCreated":"2017-07-17 11:20:55"
      }
   ],
   "CarName":"Wired India",
   "CarProfileImage":"http:\/\/fleetdemo.amberconnect.com\/uploads\/ABBHDVSJHAS_1463574102_bg.jpg",
   "ServerCurrentTime":"2017-09-05 17:42:02",
   "ServerTimezone":"UTC",
   "ServerTz":"UTC"
 }
