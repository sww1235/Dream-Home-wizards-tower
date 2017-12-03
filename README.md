# Dream-Home-wizards-tower

## TODO

-   add chimney in center of house.
-   redo third and potentially second floor to get rid of all around walkway and move bathroom towards atrium.
-   work on lighting design more
-   rethink layer heights and levels, especially in terms of ceilings and floors.
-   rethink basement, maybe shrink down, but keep in mind space for mechanical systems.
-   add lighting pipes at ceiling level on all floors around perimeter of cutout
-   add in ceiling, 6" dropped ceiling with dark wood panels at least on ground floor.
-   think about combining floor 3 and 4 into library/lounge and adding windows
or shrinking overall footprint to allow for greater height. Probably eliminate a floor
-   Add demand column and total column for electrical calcs amperage
-   Standardize subtotals row and implement if statement for total amps cell
-   How to integrate plants/planters into ground floor. Want feeling of being in jungle.
-   Add custom wooden suspended ceilings over certain areas on ground floor,
dining and living room, have them on tracks so they can be moved around. Use light
source mini can LED lights in suspended ceiling. want to not have "grid" look,
potentially have uplights/indirect light either shining through boards, or
bouncing off ceiling
-   ~~add more windows, especially to bathrooms~~
-   ~~North is oriented towards elevator~~
-   ~~move entrance to south west side~~
-   ~~add patio along east side of house~~
-   ~~add more windows into east wall of house~~
-   ~~put workshop area by elevator and combine half of -1 and -2 to give more ceiling height.~~
-   ~~change wall doors to tracked style~~
-   ~~On floors 1 and 2, have hallway on outside with interior windows in bedrooms~~

## Floor space planning

Area of circle 𝜋R²

-   Ground floor is 18' radius ==> 1,017.87 ft²
-   First floor is 17'3" radius w/ 6' radius hole ==> 821.7 ft²
-   Second floor is 16'6" radius w/ 6' radius hole ==> 742.2 ft²
-   Third floor is 15'3" radius w/ 6' radius hole ==> 617.5 ft²
-   Fourth floor is 15' radius w/ 6' radius hole ==> 593.8 ft²

Total 3793 sq ft

## General Description

House is sited so that the elevator shaft is facing north. The elevator shaft is
embedded in a hill with the majority of the house with southern exposure.

general style is a combination between medieval and modern. Lots of slate and
wood, but open plan layouts and not a lot of walls.

HVAC is 4 pipe system with localized ZCUs + zoned radiant heat, as well as a
global air recirculation/filtration/humidification system. Also allows for
adding local components to HVAC loop such as water cooled computers or mini
ZCUs.

Lots of greenery and hanging plants/vines on walls. Some used for partitions.

Bathrooms on outside of house have windows

## Lighting stuff

Primary illumination on ground floor is provided by
[WL 72º RGBW LED](https://www.thelightsource.com/products/wl-series-led-fixture-109)
fixtures (12 per 20A 120V circuit)

Secondary illumination in center of ground floor provided by either
[RD 72º RGBW LED](https://www.thelightsource.com/products/rd-series-led-fixtures-137) or
[WL 72º RGBW LED](https://www.thelightsource.com/products/wl-series-led-fixture-109)
fixtures (12 per 20A 120V circuit)

Additional RGBW tape under the lip of the stairs/RGBW led spots mounted on the
wire of the railings.

For other floors and providing additional illumination on ground floor (or
replacing the above depending on cost), are custom built RGBAW led fixtures.
These contain an arduino and sensors and use POE for data and power. Sensors
include:

-   Thermal (wet and dry bulb)
-   humidity
-   air quality (co2, o2, co, other polutants and gasses, ideally a wide spectrum sensor)
-   presence detection (Ultrasonic, infrared, radar)
-   light levels

They might also contain additional connections for switches or door/window
position sensors.

## General Technology

-   in wall vacuum system

### Radio

-   UHF commerical MotoTrbo repeater
-   2M + 70cm + 1.25M amateur repeaters

-   HF radio


## Network Planning

Datacenter in basement. Dual pfSense routers in failover mode. At least two
different fiber lines from different carriers, as well as a satelite link.

Central fiber trunk runs up in mechanical space near kitchen, with at least one
POE managed switch on each floor.

Distribution cable is carried in trays that run in the beam interstitial space.

Each light switch and custom light needs a POE network port. Also every universe
of DMX needs a network port.

## Outlet planning

each "room" needs a lighting outlet which will be manually switched with remote
control posibilities. This will be used for an LED floodlight as a backup and to
satisfy NEC requirements.

2-3 additional lighting circuits per floor

### Ground floor

2 lighting circuits in ceiling for WL lights, at least 2 more circuits in
ceiling for other stuff like powered speakers, etc.

Bathroom outlet and lighting circuit

## Appliances

### Commerical Option
-   Hobart LXeR dishwasher
-   Hobart HEC5D convection oven

### Residential Option

-   GE Café French Door Convection Wall Oven

## Ground floor

Ground floor is open plan kitchen/living room/dining room. Has central circular
fireplace with circular suspended chimney above it. This goes over floor 4 to
avoid interfering with the lighting truss. With removable supports connected to
fireplace. Fireplace is wood burning.

all furniture/appliances are on casters to allow for flexibility, with plug and
cord connected appliances and electronics connected to plugs in the ceiling.

Kitchen is industrial and all electric.

Free space can be utilized for workspace if needed

Has powder room.

## Floor 1

Master bedroom and office, potentially small powder room depending on
convenience of floor 2 bathroom

## Floor 2

Living room, a little more medieval/comfortable with chairs and sofas, large
bathroom to serve first and third floors, potentially part of library

## Floor 3

Second bedroom/third bedroom and powder room?

## Floor 4

library, observatory, potentially have a loft or catwalk in the middle of the
room over the beams for the hoist motors. Also has the power and data
connections for the truss equipment and any other cord/hose drops in the center
of the house.

## Floor -1

Has a guest suite as well as a workshop, home theatre and storage.

## Floor -2

Has datacenter and electrical distribution gear + storage. Workshop may extend
to this floor.

## Floor -3

Has HVAC equipment (chillers, boilers, heat pumps etc) for both the house and
the datacenter. Also has any potential water/sewage treatment and storage
equipment. (gray water, well, septic etc, rain water catchment, etc)
