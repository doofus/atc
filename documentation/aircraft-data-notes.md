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
- `speed.cruiseM` : 440 kts @ FL400 = 0.77M
- `speed.max` : 470 kts @ FL400 = 0.82M [Antonov](http://www.antonov.com/aircraft/passenger-aircraft/an-148/an-148-aircraft-family-performan)
- `speed.maxM` : unavailable, left as null
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A306](../assets/aircraft/a306.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 8
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : 0.82M @ FL370 = 470
- `speed.maxM` : left as 0.82, [EASA TCDS](https://www.easa.europa.eu/system/files/dfu/TCDS_EASA_A_172_AIRBUS_A300_A310_A300-600_Iss_01_20140430.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A310](../assets/aircraft/a310.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.84M @ FL400 = 482
- `speed.maxM` : left as 0.84, [EASA TCDS](https://www.easa.europa.eu/system/files/dfu/TCDS_EASA_A_172_AIRBUS_A300_A310_A300-600_Iss_01_20140430.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A318](../assets/aircraft/a318.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : 0.82M @ FL410 = 470
- `speed.maxM` : updated to 0.82, [FAA TCDS A28NM Rev. 24](http://www.airweb.faa.gov/Regulatory_and_Guidance_Library/rgMakeModel.nsf/0/57529f07d8f6e3b58625800d0057c1d4/$FILE/A28NM_Rev24.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A319](../assets/aircraft/a319.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 6.5
- `rate.decelerate` : unavailable, left as 4
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
- `speed.max` : 0.82M @ FL410 = 470
- `speed.maxM` : updated to 0.82, [FAA TCDS A28NM Rev. 24](http://www.airweb.faa.gov/Regulatory_and_Guidance_Library/rgMakeModel.nsf/0/57529f07d8f6e3b58625800d0057c1d4/$FILE/A28NM_Rev24.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A332](../assets/aircraft/a332.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 8
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 3.5
- `speed.max` : 0.86M @ FL430 = 493
- `speed.maxM` : updated to 0.86, [Airbus A332 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a330family/a330-200/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A333](../assets/aircraft/a333.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 8
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 3.5
- `speed.max` : 0.86M @ FL410 = 493
- `speed.maxM` : updated to 0.86, [Airbus A333 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a330family/a330-300/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A342](../assets/aircraft/a342.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.86M @ FL430 = 493
- `speed.maxM` : updated to 0.86, [Airbus A342 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a340family/a340-200/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A343](../assets/aircraft/a343.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.86M @ FL430 = 493
- `speed.maxM` : updated to 0.86, [Airbus A343 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a340family/a340-300/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A345](../assets/aircraft/a345.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.86M @ FL430 = 493
- `speed.maxM` : updated to 0.86, [Airbus A345 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a340family/a340-500/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A346](../assets/aircraft/a346.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : 0.86M @ FL430 = 493
- `speed.maxM` : updated to 0.86, [Airbus A346 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a340family/a340-600/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A359](../assets/aircraft/a359.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : 0.89M @ FL430 = 511
- `speed.maxM` : updated to 0.89, [Airbus ACJ350 Specifications](http://www.airbus.com/aircraftfamilies/corporate/acj-family/acj350/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A388](../assets/aircraft/a388.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 10
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 4
- `speed.cruise` : 0.85M @ FL430 = 488
- `speed.max` : 0.89M @ FL430 = 511
- `speed.maxM` : updated to 0.89, [Airbus A380 Specifications](http://www.airbus.com/aircraftfamilies/passengeraircraft/a380family/specifications/)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [AN12](../assets/aircraft/an12.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as null
- `rate.accelerate` : unavailable, left as 5
- `rate.decelerate` : unavailable, left as 4
- `speed.cruiseM` : 310 kts @ FL330 = 0.533M
- `speed.max` : updated to 348, [Global Security](http://www.globalsecurity.org/military/world/russia/an-12-specs.htm)
- `speed.maxM` : 348 kts @ FL330 = 0.598
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [AN24](../assets/aircraft/an24.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as null
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 4
- `speed.cruiseM` : 240 kts @ FL280 = 0.404M
- `speed.max` : unavailable, left as 269
- `speed.maxM` : 269 kts @ FL280 = 0.452M
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [AN72](../assets/aircraft/an72.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as null
- `rate.accelerate` : unavailable, left as 8
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : updated to 378, [Wikipedia](https://en.wikipedia.org/wiki/Antonov_An-72)
- `speed.maxM` : 378 kts @ FL380 = 0.66M
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [AT43](../assets/aircraft/at43.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 3
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 6
- `speed.cruiseM` : 255 kts @ FL250 = 0.424M
- `speed.max` : updated to 266, [ATR 42-300 Brochure](http://www.atraircraft.com/products_app/media/pdf/FAMILY_septembre2014.pdf)
- `speed.maxM` : 266 kts @ FL250 = 0.442M
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [AT45](../assets/aircraft/at45.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 3
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 6
- `speed.cruiseM` : 255 kts @ FL260 = 0.424M
- `speed.max` : updated to 300, [ATR 42-500 Brochure](http://www.atraircraft.com/products_app/media/pdf/FAMILY_septembre2014.pdf)
- `speed.maxM` : 300 kts @ FL260 = 0.50M
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [AT72](../assets/aircraft/at72.json)

**Serveral varaiants of the ATR 72 exist.  The ATR 72-500 model is used here**

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 3
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 5
- `speed.cruiseM` : 275 kts @ FL250 = 0.457M
- `speed.max` : updated to 275, [ATR 72-500 Brochure](http://www.atraircraft.com/products_app/media/pdf/FAMILY_septembre2014.pdf)
- `speed.maxM` : 275 kts @ FL250 = 0.457M
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [AT76](../assets/aircraft/at76.json)

No entry exists in the Eurocontrol Aircraft Performance Database.  Data from
the AT72 is used and augmented by the [ATR 72-600 Brochure](http://www.atraircraft.com/products_app/media/pdf/FAMILY_septembre2014.pdf).

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 3
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 5
- `speed.cruiseM` : 275 kts @ FL250 = 0.457M
- `speed.max` : updated to 275, [ATR 72-600 Brochure](http://www.atraircraft.com/products_app/media/pdf/FAMILY_septembre2014.pdf)
- `speed.maxM` : 275 kts @ FL250 = 0.457M
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B712](../assets/aircraft/b712.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 5
- `rate.decelerate` : unavailable, left as 5
- `speed.max` : unavailable, set to cruise speed
- `speed.maxM` : unavailable, set to cruise speed
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B722](../assets/aircraft/b722.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 5
- `speed.max` : 0.90M @ FL400 = 516 kts
- `speed.maxM` : updated to 0.90 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_727#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B732](../assets/aircraft/b732.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 5
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.82M @ FL370 = 470 kts
- `speed.maxM` : updated to 0.82 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_737#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B733](../assets/aircraft/b733.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.82M @ FL370 = 470 kts
- `speed.maxM` : updated to 0.82 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_737_Classic#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B734](../assets/aircraft/b734.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 8
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.82M @ FL370 = 470 kts
- `speed.maxM` : updated to 0.82 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_737_Classic#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B735](../assets/aircraft/b735.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 5
- `speed.max` : 0.82M @ FL370 = 470 kts
- `speed.maxM` : updated to 0.82 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_737_Classic#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B736](../assets/aircraft/b736.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.825M @ FL410 = 473 kts
- `speed.maxM` : updated to 0.825 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_737_Next_Generation#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B737](../assets/aircraft/b737.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 8
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.825M @ FL410 = 473 kts
- `speed.maxM` : updated to 0.825 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_737_Next_Generation#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B738](../assets/aircraft/b738.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.825M @ FL410 = 473 kts
- `speed.maxM` : updated to 0.825 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_737_Next_Generation#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B739](../assets/aircraft/b739.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.825M @ FL410 = 473 kts
- `speed.maxM` : updated to 0.825 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_737_Next_Generation#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B741](../assets/aircraft/b741.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 10
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 2
- `speed.max` : 0.92M @ FL450 = 528 kts
- `speed.maxM` : updated to 0.92 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_747#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B742](../assets/aircraft/b742.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 10
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 2
- `speed.max` : 0.92M @ FL450 = 528 kts
- `speed.maxM` : updated to 0.92 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_747#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B744](../assets/aircraft/b744.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 10
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 2
- `speed.max` : 0.92M @ FL450 = 528 kts
- `speed.maxM` : updated to 0.92 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_747#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B748](../assets/aircraft/b748.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 10
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 3
- `speed.max` : 0.90M @ FL450 = 516 kts
- `speed.maxM` : updated to 0.90 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_747-8#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B752](../assets/aircraft/b752.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 8
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : 0.86M @ FL420 = 493 kts
- `speed.maxM` : updated to 0.86 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_757#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B753](../assets/aircraft/b753.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 8
- `rate.accelerate` : unavailable, left as 8
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : 0.86M @ FL420 = 493 kts
- `speed.maxM` : updated to 0.86 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_757#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B762](../assets/aircraft/b762.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : updated to 486 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_767#Specifications)
- `speed.maxM` : 486 kts @ FL390 = 0.847M
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B763](../assets/aircraft/b763.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : updated to 486 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_767#Specifications)
- `speed.maxM` : 486 kts @ FL390 = 0.847M
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B764](../assets/aircraft/b764.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 8
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : updated to 486 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_767#Specifications)
- `speed.maxM` : 486 kts @ FL390 = 0.847M
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B772](../assets/aircraft/b772.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 3.5
- `speed.max` : 0.89M @ FL430 = 511 kts
- `speed.maxM` : updated to 0.89 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_777#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B773](../assets/aircraft/b773.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 5.5
- `rate.decelerate` : unavailable, left as 3.2
- `speed.max` : 0.89M @ FL430 = 511 kts
- `speed.maxM` : updated to 0.89 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_777#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B74S](../assets/aircraft/b74s.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 3
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 2
- `speed.max` : updated to 528, [Wikipedia](https://en.wikipedia.org/wiki/Boeing_747SP#Specifications)
- `speed.maxM` : updated to 0.92, [Wikipedia](https://en.wikipedia.org/wiki/Boeing_747SP#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B77L](../assets/aircraft/b77l.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 3.5
- `speed.max` : 0.89M @ FL431 = 511 kts
- `speed.maxM` : updated to 0.89 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_777#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B77W](../assets/aircraft/b77w.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 9
- `rate.accelerate` : unavailable, left as 6
- `rate.decelerate` : unavailable, left as 3.5
- `speed.max` : 0.89M @ FL431 = 511 kts
- `speed.maxM` : updated to 0.89 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_777#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B788](../assets/aircraft/b788.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 4
- `speed.max` : 0.89M @ FL430 = 511 kts
- `speed.maxM` : updated to 0.89 [Wikipedia](https://en.wikipedia.org/wiki/Boeing_787_Dreamliner#Specifications)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [B789](../assets/aircraft/b789.json)

** No entry in Eurocontrol Database.  Reusing B788 data. **
