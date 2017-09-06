Trips History
=============

Amber connect logs every trip with comprehensive details of distance, time, speed and fuel spent at close of every trip based on ignition status of the vehicle. This api end point allows you to access the trips of a specific vehicle/Device.

This method returns a list of all trips that a given device/Vehcile has taken.  This will not include trips that have not yet been completed.


Request
+++++++

.. code-block:: json

      POST hhttp://dev.amberconnect.com/AmberConnectApp/public/v2.4/openapi/gettrips
      Accept: application/json

* `DeviceOffset` - Mandatory, Default=0
* `AmberAuthToken` - Mandatory, Amber device's unique QR code.
* `APIKey` - Mandatory
* `Filter` - Optional parameter. Possible value is "Custom"
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
   "GeoRouteStatus":"ON",
   "CarName":"Wired India",
   "CarProfileImage":"http:\/\/fleetdemo.amberconnect.com\/uploads\/ABBHDVSJHAS_1463574102_bg.jpg",
   "Trips":[
      {
         "Id":"LJVPI8MYN3GA20170407054524",
         "TripStartPoint":"Avinashi Road, Coimbatore, TN",
         "TripEndPoint":"Gman",
         "StartTime":"2017-04-07 05:45:25",
         "EndTime":"2017-04-07 06:31:48",
         "InterParkedDuration":"0",
         "DurationSeconds":"2783",
         "DriverId":"",
         "ParkedTimeDuration":"",
         "Distance":"16.1",
         "Fuel":"1.81",
         "DriverName":[

         ],
         "TopSpeed":"60",
         "GeoRouteStatus":"N",
         "Duration":"0.77",
         "Mileage":"8.94",
         "Idle":"0.29",
         "CostPerPrice":"0.11242236024845",
         "IdleTimeFuelPrice":"0.62",
         "TripType":"",
         "FuelConume":"1.8",
         "OdometerReading":"326032",
         "LatLong":{
            "StartPointLat":"11.024013333333",
            "StartPointLong":"77.006337777778",
            "EndPointLat":"11.02111",
            "EndPointLong":"77.019937777778",
            "MapsImage":"http:\/\/maps.googleapis.com\/maps\/api\/staticmap?size=300x300\u0026path=weight:7%7Ccolor:0x003366%7Cenc:achbAqh_uMtaB`zI]iA[cBSuB]gEo@oGMeBg@q@iCZqCPi@CMUMwHCUFaAbCwBpDoCvDkCzDwCxBmBzCuBzCiBhCqAj@c@fAe@^iBKyAWkBm@kCHeBn@Ih@CbBShAEn@?bBMHSWmB[kEm@eHc@iEaA}FuAuEo@}AkAgCeBaDuAqC{AgCsB{DcCoDcIyJ}BgDwAoCyABBH`AKeAaC}@gBiGkNqCuFaAyAQKmFsGuCyDiEaE{FqD}MqHuAq@c@c@}CkFwAeEeCgK]{DU{F_@mGeBqFuAqDy@qCYoC[uD_@_Dm@_DUsBK_ASoD}A_Oo@aJQuD]}Mo@uLXg@bCKxC?jCJhCSzBw@fDk@|Bk@Ec@gA{F\u0026markers=size:mid:http:\/\/goo.gl\/4YM8wr|11.024013333333,77.006337777778\u0026markers=size:mid:http:\/\/goo.gl\/VHRSbR|11.02111,77.019937777778"
         },
         "Polyline":"achbAqh_uMtaB`zI]iA[cBSuB]gEo@oGMeBg@q@iCZqCPi@CMUMwHCUFaAbCwBpDoCvDkCzDwCxBmBzCuBzCiBhCqAj@c@fAe@^iBKyAWkBm@kCHeBn@Ih@CbBShAEn@?bBMHSWmB[kEm@eHc@iEaA}FuAuEo@}AkAgCeBaDuAqC{AgCsB{DcCoDcIyJ}BgDwAoCyABBH`AKeAaC}@gBiGkNqCuFaAyAQKmFsGuCyDiEaE{FqD}MqHuAq@c@c@}CkFwAeEeCgK]{DU{F_@mGeBqFuAqDy@qCYoC[uD_@_Dm@_DUsBK_ASoD}A_Oo@aJQuD]}Mo@uLXg@bCKxC?jCJhCSzBw@fDk@|Bk@Ec@gA{F",
         "ShowDetailsFlag":"Y",
         "Warning":{
            "HardBrakes":"0",
            "SuddenAccels":"1",
            "Speeding":"0",
            "AlertPoints":[
               {
                  "Type":"SuddenAccels",
                  "Latitude":"11.002523333333",
                  "Longitude":"76.967182222222",
                  "AlertTime":"2017-04-07 06:03:32"
               }
            ]
         },
         "TripIntermediatePoints":[

         ]
      },
      {
         "Id":"LJVPI8MYN3GA20170406091911",
         "TripStartPoint":"Avinashi Road, Coimbatore, TN",
         "TripEndPoint":"Gman",
         "StartTime":"2017-04-06 09:19:11",
         "EndTime":"2017-04-06 09:32:40",
         "InterParkedDuration":"0",
         "DurationSeconds":"809",
         "DriverId":"",
         "ParkedTimeDuration":"72765",
         "Distance":"5.4",
         "Fuel":"0.45",
         "DriverName":[

         ],
         "TopSpeed":"55",
         "GeoRouteStatus":"N",
         "Duration":"0.22",
         "Mileage":"12",
         "Idle":"0",
         "CostPerPrice":"0.083333333333333",
         "IdleTimeFuelPrice":"0",
         "TripType":"",
         "FuelConume":"0.45",
         "OdometerReading":"326027",
         "LatLong":{
            "StartPointLat":"11.009861111111",
            "StartPointLong":"76.980586666667",
            "EndPointLat":"11.02139",
            "EndPointLong":"77.019768888889",
            "MapsImage":"http:\/\/maps.googleapis.com\/maps\/api\/staticmap?size=300x300\u0026path=weight:7%7Ccolor:0x003366%7Cenc:sjebAsgztMVd@Hc@g@uAyD{H}AuDkBeEyAqCaB_CkCiDgC{CsAgBiCsCoDwCaTuLcCiByAkCmBkE}BmJ[gB_@cDa@}Km@gEcBaFgBwEw@cEe@sF_AmGi@uF_@sFc@qFo@_F[uEWyFW{LUcE]iERsAvBGbCA`DPbD_@rBq@|G}AS{Ae@kCg@u@_@b@\u0026markers=size:mid:http:\/\/goo.gl\/4YM8wr|11.009861111111,76.980586666667\u0026markers=size:mid:http:\/\/goo.gl\/VHRSbR|11.02139,77.019768888889"
         },
         "Polyline":"sjebAsgztMVd@Hc@g@uAyD{H}AuDkBeEyAqCaB_CkCiDgC{CsAgBiCsCoDwCaTuLcCiByAkCmBkE}BmJ[gB_@cDa@}Km@gEcBaFgBwEw@cEe@sF_AmGi@uF_@sFc@qFo@_F[uEWyFW{LUcE]iERsAvBGbCA`DPbD_@rBq@|G}AS{Ae@kCg@u@_@b@",
         "ShowDetailsFlag":"Y",
         "Warning":{
            "HardBrakes":"0",
            "SuddenAccels":"0",
            "Speeding":"0",
            "AlertPoints":[

            ]
         },
         "TripIntermediatePoints":[

         ]
      },
      {
         "Id":"LJVPI8MYN3GA20170406075354",
         "TripStartPoint":"Gman",
         "TripEndPoint":"Avinashi Road, Coimbatore, TN",
         "StartTime":"2017-04-06 07:53:54",
         "EndTime":"2017-04-06 08:23:37",
         "InterParkedDuration":"0",
         "DurationSeconds":"1783",
         "DriverId":"",
         "ParkedTimeDuration":"3334",
         "Distance":"6.1",
         "Fuel":"0.51",
         "DriverName":[

         ],
         "TopSpeed":"64",
         "GeoRouteStatus":"N",
         "Duration":"0.5",
         "Mileage":"12",
         "Idle":"0",
         "CostPerPrice":"0.083606557377049",
         "IdleTimeFuelPrice":"0",
         "TripType":"",
         "FuelConume":"0.50833333333333",
         "OdometerReading":"326021",
         "LatLong":{
            "StartPointLat":"11.021026666667",
            "StartPointLong":"77.019564444444",
            "EndPointLat":"11.009866666667",
            "EndPointLong":"76.980613333333",
            "MapsImage":"http:\/\/maps.googleapis.com\/maps\/api\/staticmap?size=300x300\u0026path=weight:7%7Ccolor:0x003366%7Cenc:kpgbAg{auMbh@vdEz@nAbBrBfAjAlAtAjBnChAtB|C~GnBvD|E`KrCvEpIrKvChEdBtC|AvC{EcIuDeFwEaGuDkF{AaCWDUXb@D\u0026markers=size:mid:http:\/\/goo.gl\/4YM8wr|11.021026666667,77.019564444444\u0026markers=size:mid:http:\/\/goo.gl\/VHRSbR|11.009866666667,76.980613333333"
         },
         "Polyline":"kpgbAg{auMbh@vdEz@nAbBrBfAjAlAtAjBnChAtB|C~GnBvD|E`KrCvEpIrKvChEdBtC|AvC{EcIuDeFwEaGuDkF{AaCWDUXb@D",
         "ShowDetailsFlag":"Y",
         "Warning":{
            "HardBrakes":"0",
            "SuddenAccels":"0",
            "Speeding":"0",
            "AlertPoints":[

            ]
         },
         "TripIntermediatePoints":[

         ]
      },
      {
         "Id":"LJVPI8MYN3GA20170406063514",
         "TripStartPoint":"Ellaithottam Road, Coimbatore, TN",
         "TripEndPoint":"Masakalipalayam Link Road, Coimbatore, TN",
         "StartTime":"2017-04-06 05:26:04",
         "EndTime":"2017-04-06 06:53:59",
         "InterParkedDuration":"626",
         "DurationSeconds":"4649",
         "DriverId":"",
         "ParkedTimeDuration":"3595",
         "Distance":"23.8",
         "Fuel":"2.15",
         "DriverName":[

         ],
         "TopSpeed":"58",
         "GeoRouteStatus":"N",
         "Duration":"1.29",
         "Mileage":"9.31",
         "Idle":"0.09",
         "CostPerPrice":"0.19317617866005",
         "IdleTimeFuelPrice":"0.19",
         "TripType":"",
         "FuelConume":"2.1333333333333",
         "OdometerReading":"325997",
         "LatLong":{
            "StartPointLat":"11.028803333333",
            "StartPointLong":"77.006666666667",
            "EndPointLat":"11.02089",
            "EndPointLong":"77.01912",
            "MapsImage":"http:\/\/maps.googleapis.com\/maps\/api\/staticmap?size=300x300\u0026path=weight:7%7Ccolor:0x003366%7Cenc:_aibAsj_uMyqCtkAi@mBYa@{CyIwAoD_BeDiC}BoAoDmBkI{@}BaD}F{AgDmAaDa@i@{Ds@mBoCaBoCuDmIoBiDcNiTmCoDkAsDAoCp@?pALfKXtFHzEXnELpD@zDFpEZfA@lALdA@jOn@dDPrEr@hJ`B|EP`F@dDWjHs@hGOrFGbEOfF[jDm@hA[bAE|AWvD}@fF}AdDy@`Fu@`BOdC_@zH{@~BoAb@w@vBqCpByClEcHrBsDuAoEqAoDESn@k@l@Nj@pBhDrI`@x@b@BfIqBjE}@~Fw@bAj@f@jFd@`Dx@LdA|Ff@JCRkHdAeEfAsCFmCQwBHcBn@\\bKV`Md@zJJ|AhAbKx@fK^rDt@~EpAvLp@hC|DtK^jD^zJJhAt@`FbAlEtAbFxBhEl@bA`ClBbKtFnEhCzDtC|CvCjF|GlBrBdAtAbBpCrDbIlDdHxClG`B~ChCpDtDrEtD`FtCpEbBvCPd@QE_AkBeB}CeC}D_J_LeCsDuA_CYf@w|@weAs@g@aCwDcBwD}BmJ]kC_@oDo@{MsAkEaCuGw@{C]}EcB}LYeCi@uIkAyKSiDe@{KQwJg@gHM}@?o@^c@bCInJCr@KdD{@vDu@bAm@]oB\u0026markers=size:mid:http:\/\/goo.gl\/4YM8wr|11.028803333333,77.006666666667\u0026markers=size:mid:http:\/\/goo.gl\/VHRSbR|11.02089,77.01912\u0026markers=size:mid:http:\/\/goo.gl\/4YM8wr|11.028803333333,77.006666666667\u0026markers=size:mid:http:\/\/goo.gl\/VHRSbR|11.02089,77.01912"
         },
         "Polyline":"_aibAsj_uMyqCtkAi@mBYa@{CyIwAoD_BeDiC}BoAoDmBkI{@}BaD}F{AgDmAaDa@i@{Ds@mBoCaBoCuDmIoBiDcNiTmCoDkAsDAoCp@?pALfKXtFHzEXnELpD@zDFpEZfA@lALdA@jOn@dDPrEr@hJ`B|EP`F@dDWjHs@hGOrFGbEOfF[jDm@hA[bAE|AWvD}@fF}AdDy@`Fu@`BOdC_@zH{@~BoAb@w@vBqCpByClEcHrBsDuAoEqAoDESn@k@l@Nj@pBhDrI`@x@b@BfIqBjE}@~Fw@bAj@f@jFd@`Dx@LdA|Ff@JCRkHdAeEfAsCFmCQwBHcBn@\\bKV`Md@zJJ|AhAbKx@fK^rDt@~EpAvLp@hC|DtK^jD^zJJhAt@`FbAlEtAbFxBhEl@bA`ClBbKtFnEhCzDtC|CvCjF|GlBrBdAtAbBpCrDbIlDdHxClG`B~ChCpDtDrEtD`FtCpEbBvCPd@QE_AkBeB}CeC}D_J_LeCsDuA_CYf@w|@weAs@g@aCwDcBwD}BmJ]kC_@oDo@{MsAkEaCuGw@{C]}EcB}LYeCi@uIkAyKSiDe@{KQwJg@gHM}@?o@^c@bCInJCr@KdD{@vDu@bAm@]oB",
         "ShowDetailsFlag":"Y",
         "Warning":{
            "HardBrakes":"0",
            "SuddenAccels":"1",
            "Speeding":"0",
            "AlertPoints":[
               {
                  "Type":"SuddenAccels",
                  "Latitude":"11.052293333333",
                  "Longitude":"76.994391111111",
                  "AlertTime":"2017-04-06 05:42:52"
               }
            ]
         },
         "TripIntermediatePoints":[
            {
               "Location":"Avinashi Road, Coimbatore, TN",
               "Latitude":"11.028803333333",
               "Longitude":"77.006666666667",
               "StartedNextDateTime":"2017-04-06 06:35:14",
               "DateTime":"2017-04-06 06:24:48",
               "InterTripId":"LJVPI8MYN3GA20170406052604"
            }
         ],
         "TripExistStartPoint":"Green Trends"
      }
   ],
   "DeviceCategory":"CAR",
   "DeviceType":"WGPS",
   "count":1421,
   "start":1,
   "end":15,
   "CurrencyText":"USD",
   "LastStartTime":"2017-04-01 10:15:49",
   "DistanceUnit":"Kms",
   "UserName":"",
   "ProfileImage":"",
   "ServerCurrentTime":"2017-09-05 17:22:20",
   "ServerTimezone":"UTC",
   "ServerTz":"UTC"
 }
