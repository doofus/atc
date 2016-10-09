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
- `speed.max` : unavailable, left as 484
- `speed.maxM` : left as 0.82, [EASA TCDS](https://www.easa.europa.eu/system/files/dfu/TCDS_EASA_A_172_AIRBUS_A300_A310_A300-600_Iss_01_20140430.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A310](../assets/aircraft/a310.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 4
- `rate.decelerate` : unavailable, left as 3
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : unavailable, left as 487
- `speed.maxM` : left as 0.84, [EASA TCDS](https://www.easa.europa.eu/system/files/dfu/TCDS_EASA_A_172_AIRBUS_A300_A310_A300-600_Iss_01_20140430.pdf)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true

## [A318](../assets/aircraft/a318.json)

- `category.srs` : left as 3, agrees with [FAA JO 7110.65W](https://www.faa.gov/documentLibrary/media/Order/ATC.pdf)
- `category.lahso` : unavailable, left as 7
- `rate.accelerate` : unavailable, left as 7
- `rate.decelerate` : unavailable, left as 4
- `speed.min` : back-calculated from Approach Speed
- `speed.max` : updated to 467, [BA](http://www.britishairways.com/en-gb/information/about-ba/fleet-facts/airbus-318-100
)
- `capability.ils` : unavailable, left as true
- `capability.fix` : unavailable, left as true
