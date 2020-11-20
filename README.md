# CourtVisionPH - UAAP Season 81 FIBA LiveStats Shot Chart Data

Includes information found in the Shot Chart data of FIBA LiveStats:
- location (origin is the center of the basket)
    - **x** - distance (10 cm/unit) from center of basket along x (horizontal) axis, right is positive
    - **y** - distance (10 cm/unit) from the center of the basket along y (vertical) axis, up is positive
- **points** - 2 or 3
- **made** - 1 is made, 0 is missed
- **shot_type** - type of shot taken
- player & team information
    - **player** - name of player
    - **num** - number of player
    - **team** - team of player
    - **opponent** - opponent team in the game
- **date** - date when game was played
- **venue** - where the game was played

## Notes
x and y are in 10 cm intervals. 1 unit of x or y = 10 centimeters (0.1 meters). Meaning, a point with coordinates (10, 10) is 100cm (10 * 10cm) to the right and 100 cm away from the basket.

Original data extracted from [FIBA LiveStats](https://www.fibalivestats.com/).

## Extraction done by scraping data from FIBA LiveStats and mapping them to a half-court
![ETL of data](/img/etl.png)

## Sample analysis and visualizations
Distances of made three-pointers
![Distances of three-pointers](/img/Day02-Lines.png)

Range map of UP Fighting Maroons
![Range map of UP Fighting Maroons](/img/Day04-Hexagons-UP.png)

Spatial basis vectors using NMF and KDE
![Spatial basis vectors using NMF and KDE](/img/nmf.png)

![Creative Commons License BY-SA](https://i.creativecommons.org/l/by-sa/4.0/80x15.png)

Except when explicitly stated otherwise, this work and its contents is licensed under a <a rel="license" href="https://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)</a>.<br>

