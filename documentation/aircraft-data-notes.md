---
title: Notes on Aircraft Data
---
[back to index](index.md)

# Data Sources

[The Eurocontrol Aircraft Performance Database](https://contentzone.eurocontrol.int/aircraftperformance/default.aspx?)
is used as the primary source for techincal data and performance data for
aircraft types.  
Any gaps in the data from the Eurocontrol Aircraft Performance Database should
then be sourced from the aircraft manufacturer and annotated in this file.  
If data from the manufacturer is not available, then another source may be used.
This source should also be annotated in this file.  
If any gaps are still unresolved, then they should be annotated in this file.

## Climb / Descent Rates

Climb rates (`rate.climb`)should use the climb rate given for the "Climb to FL150" phase of flight.
Descent rates (`rate.descent`) should use the descent rate given for the "Approach" phase of flight.

# Data Format

Please see the [Aircraft Format](aircraft_format.md) documentation for
descriptions of the data fields.

# Aircraft

## [A124](../assets/aircraft/a124.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as null
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 2
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : updated to 467, [Wikipedia](https://en.wikipedia.org/wiki/Antonov_An-124_Ruslan)
- `speed.maxM` : unavailable, left as null
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A148](../assets/aircraft/a148.json)

**The Eurocontrol Database has no entry for the Antonov An-148.**

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `weightclass` : updated to "M", [doc8643.com](https://doc8643.com/aircraft/A148)
- `category.srs` : unavailable, left as null
- `category.lahso` : unavailable, left as null
- `category.recat` : unavailable, left as "D"
- `ceiling` : updated to 40000, [Antonov](http://www.antonov.com/aircraft/passenger-aircraft/an-148/an-148-aircraft-family-performan)
- `rate.climb` : updated to 2500, [doc8643.com](https://doc8643.com/aircraft/A148)
- `rate.descent` : updated to 2000, [doc8643.com](https://doc8643.com/aircraft/A148)
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 2
- `runway.takeoff` : updated to 1.885, [Antonov](http://www.antonov.com/aircraft/passenger-aircraft/an-148/an-148-aircraft-family-performan)
- `runway.landing` : unavilable, left as 2.100
- `speed.min`: unavailable, left as 90
- `speed.landing` : unavailable, left as 111
- `speed.cruise` : left as 440, [doc8643.com](https://doc8643.com/aircraft/A148)
- `speed.cruiseM` : unavailable, left as null
- `speed.max` : left as 470, [Antonov](http://www.antonov.com/aircraft/passenger-aircraft/an-148/an-148-aircraft-family-performan)
- `speed.maxM` : unavailable, left as null
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A306](../assets/aircraft/a306.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 8
- `rate.decelerate` : unavailable, left as 4
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.82M @ FL370 = 470
- `speed.maxM` : left as 0.82, [EASA TCDS](https://www.easa.europa.eu/system/files/dfu/TCDS_EASA_A_172_AIRBUS_A300_A310_A300-600_Iss_01_20140430.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A310](../assets/aircraft/a310.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 3
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.84M @ FL400 = 482
- `speed.maxM` : left as 0.84, [EASA TCDS](https://www.easa.europa.eu/system/files/dfu/TCDS_EASA_A_172_AIRBUS_A300_A310_A300-600_Iss_01_20140430.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A318](../assets/aircraft/a318.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 4
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.82M @ FL410 = 470
- `speed.maxM` : updated to 0.82, [FAA TCDS A28NM Rev. 24](http://www.airweb.faa.gov/Regulatory_and_Guidance_Library/rgMakeModel.nsf/0/57529f07d8f6e3b58625800d0057c1d4/$FILE/A28NM_Rev24.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A319](../assets/aircraft/a319.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 6.5
- `rate.decelerate` : unavailable, left as 4
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.82M @ FL390 = 470
- `speed.maxM` : updated to 0.82, [FAA TCDS A28NM Rev. 24](http://www.airweb.faa.gov/Regulatory_and_Guidance_Library/rgMakeModel.nsf/0/57529f07d8f6e3b58625800d0057c1d4/$FILE/A28NM_Rev24.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A320](../assets/aircraft/a320.json)

**Two variants exist: A320-100 and A320-200. Very few A320-100 models exist. Assuming data pertains to A320-200.**

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 4
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.82M @ FL410 = 470
- `speed.maxM` : updated to 0.82, [FAA TCDS A28NM Rev. 24](http://www.airweb.faa.gov/Regulatory_and_Guidance_Library/rgMakeModel.nsf/0/57529f07d8f6e3b58625800d0057c1d4/$FILE/A28NM_Rev24.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A321](../assets/aircraft/a321.json)

**Two variants exist: A321-100 and A321-200. Assuming data pertains to A320-200.**

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 4
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.82M @ FL410 = 470
- `speed.maxM` : updated to 0.82, [FAA TCDS A28NM Rev. 24](http://www.airweb.faa.gov/Regulatory_and_Guidance_Library/rgMakeModel.nsf/0/57529f07d8f6e3b58625800d0057c1d4/$FILE/A28NM_Rev24.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A332](../assets/aircraft/a332.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 8
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 3.5
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.86M @ FL430 = 493
- `speed.maxM` : updated to 0.86, [Airbus A332 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a330family/a330-200/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A333](../assets/aircraft/a333.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 8
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 3.5
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.86M @ FL410 = 493
- `speed.maxM` : updated to 0.86, [Airbus A333 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a330family/a330-300/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A342](../assets/aircraft/a342.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 3
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.86M @ FL430 = 493
- `speed.maxM` : updated to 0.86, [Airbus A342 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a340family/a340-200/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A343](../assets/aircraft/a343.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 3
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.86M @ FL430 = 493
- `speed.maxM` : updated to 0.86, [Airbus A343 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a340family/a340-300/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A345](../assets/aircraft/a345.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 3
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.86M @ FL430 = 493
- `speed.maxM` : updated to 0.86, [Airbus A345 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a340family/a340-500/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A346](../assets/aircraft/a346.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 4
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : 0.86M @ FL430 = 493
- `speed.maxM` : updated to 0.86, [Airbus A346 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a340family/a340-600/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A359](../assets/aircraft/a359.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 4
- `speed.min` : back-calculated from Approach Speed
- `speed.cruise` : 0.85M @ FL430 = 488
- `speed.max` : 0.89M @ FL430 = 511
- `speed.maxM` : updated to 0.89, [Airbus ACJ350 Specifications](http://www.airbus.com/aircraftfamilies/corporate/acj-family/acj350/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A388](../assets/aircraft/a388.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 10
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 4
- `speed.min` : back-calculated from Approach Speed
- `speed.cruise` : 0.85M @ FL430 = 488
- `speed.max` : 0.89M @ FL430 = 511
- `speed.maxM` : updated to 0.89, [Airbus A380 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a380family/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true
