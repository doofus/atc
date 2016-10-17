---
title: Aircraft Format Wiki
---
[back to index](index.html)

[!image](http://puu.sh/o6oee/00a63d977a.png)

[The Eurocontrol Aircraft Performance Database](https://contentzone.eurocontrol.int/aircraftperformance/default.aspx?)
is used as the primary source for techincal data and performance data for
aircraft types.  
Any gaps in the data from the Eurocontrol Aircraft Performance Database should
then be sourced from the aircraft manufacturer and annotated in [aircraft-data-notes.md](./aircraft-data-notes.md).
If data from the manufacturer is not available, then another source may be used.
This source should also be annotated in [aircraft-data-notes.md](./aircraft-data-notes.md).  
If any gaps are still unresolved, then they should be annotated in [aircraft-data-notes.md](./aircraft-data-notes.md).

## Example Aircraft File

{
  "name": "Boeing 747-400",   - Official name of the aircraft²
  "icao": "B744",             - ICAO identifier of the aircraft¹²
  "engines": {
    "number": 4,              - Number of Engines¹²
    "type": "J"               - Engines type¹² - [J = Jet / T = TurboProp / P = Piston]
  },
  "weightclass": "H",   - wake turbulence category¹²
  "category": {
    "srs": 3,           - Same Runway Separation Category¹
    "lahso": 10,        - LAHSO (land-and-hold-short) Category¹
    "recat": "B"        - Wake Turb Recategorization Category³
  },
  "ceiling": 45000,     - Service Ceiling²
  "rate": {
    "climb":      2000, - Climb Rate² (DON'T use 7110.65, its values are VERY inaccurate)
    "descent":    3000, - Descent Rate² (DON'T use 7110.65, its values are VERY inaccurate)
    "accelerate": 4,    - Accelerate Rate (your best estimate, btwn ~1-5)
    "decelerate": 2     - Decelerate Rate (your best estimate, btwn ~1-5)
  },
  "runway": {
    "takeoff": 3.352,   - Takeoff Distance Required² (km)
    "landing": 2.072    - Landing Distance Required² (km)
  },
  "speed":{
    "min":     135,   - Takeoff Speed² (V<sub>2</sub>)
    "landing": 150,   - Landing speed² (at threshold) or Approach Speed (Vat); usually 1.3 times the Stall Speed
    "cruise":  492    - Typical cruise speed², knots (a/c will fly at slower of these speeds)
    "cruiseM": 0.81,  - Typical cruise speed², mach  (a/c will fly at slower of these speeds) if unavailable, put null
    "max":     507,   - Never-Exceed speed² (Vne), knots. Fastest possible speed before structural damage.
    "maxM":    0.83   - Maximum Speed², mach. If unavailable, put null
  },
  "capability": {
    "ils": true,      - T/F: whether aircraft has ILS equipment
    "fix": true       - T/F: whether aircraft has VOR or GPS equipment
  }
}



## Notes

¹ Available in FAA JO 7110.65V, Appendix A (http://www.faa.gov/documentLibrary/media/Order/7110.65V.pdf)
² May be available from [Eurocontrol](https://contentzone.eurocontrol.int/aircraftperformance/details.aspx?), aircraft manufacturer, Wikipedia, or other sources.
³ See FAA JO 7110.659B (http://www.faa.gov/documentLibrary/media/Order/Final_Wake_Recat_Order.pdf)
  and look up aircraft's MTOW (Max Certified Gross Takeoff Weight) and wingspan. Compare those
  values to the ranges listed in FAA JO 7110.659B, "Aircraft Wake Categories" section within the
  document's "Pilot/Controller Glossary". Can be Category A, B, C, D, E, or F.
