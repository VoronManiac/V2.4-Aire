# V2.4-Aire #
Each Aire filter has a HEPA particle prefilter followed by an activated charcoal filter and is targeted at Voron 2.4 250/300/350 printers. Ideally, a pair of filters is mounted on either side of the print bed. The design is optimized for high air flow to increase the turnover rate and minimize particulate concentration. <br>

![](./images/PXL_20240910_233532594a.jpg?raw=true)

Aire uses inexpensive Eufy RoboVAC HEPA filters.  The Eufy HEPA filter sits above the 5015 blower, but sufficient space is provided between the two to prevent the blower from stalling.  The blower exhaust feeds the single piece activated carbon cartridge which attaches to the HEPA/blower section with magnets. Once loaded with charcoal, two small doors slide into place to close off the cartridge. 

As shown below, the air path in the cartridge splits into two sections, passing through a 17mm wide layer of charcoal,  and then gets collected in the output plenums.  The split path and relatively thin width of charcoal reduces blower back pressure and helps increase airflow.  Each 95mm cartridge has similar charcoal capacity compared to NeverMore DuoV5.  If additional capacity is needed, the 95mm cartridge could be redesigned to further increase the charcoal volume by lengthening it, which incidentally would *decrease* the blower back pressure even further and increase airflow.

![](./images/AirFlow.jpg?raw=true)

It is difficult to say how frequently the HEPA filter and charcoal need to be replaced without some direct particle and VOC measurements, but the pic below shows a dirty filter after 4 months of usage compared to a fresh filter. With the Zyltech ABS filament I have been running, the charcoal should last for many weeks of continuous printing.

![](./images/PXL_20240912_020730545b.jpg?raw=true)




## BOM ##
| Qty        | Item           | Comment |
|:------------- |:------------- |:----- |
|2           | Eufy RoboVac Filter 110x48x10(mm)| https://www.amazon.com/gp/product/B07F5XK5WN/ref=ppx_yo_dt_b_search_asin_title  |
|2           |GDSTIME 5015 Turbo Dual BB 24V  | https://www.amazon.com/gp/product/B0B1V6JTB8/ref=ppx_yo_dt_b_search_asin_title  |
|2      | 2-Pin 2.5mm JST Male Pin Header | like https://www.digikey.com/en/products/detail/jst-sales-america-inc./B2B-XH-A/1651045  or https://www.amazon.com/gp/product/B08YNFGYNH/ref=ppx_yo_dt_b_search_asin_title|
| 16  | M3x8 BHCS |  |
|4|M3 Half Round T Nuts|https://www.amazon.com/gp/product/B08YNFGYNH/ref=ppx_yo_dt_b_search_asin_title |
| 4 | M3 9mm washer |    |
| 12 |  M3xD5.0xL4.0 Heatset Insert | |
| 16 | N52 magnets 6mm dia x 3mm thick| | 
| 2  | 10mm Red/Black 1.5mm Dia heat shrink tubing| |
| bag | activated charcoal | |

## Printing ##

Print in ABS using standard Voron Settings: 40% infill, 4 perimeters, 5 solid bottom/top, no supports.    

A z-lift of 0.1mm seemed to reduce stringing when printing the CarbonFilter grid, but significantly increases the print time.

The CarbonFilter STL is designed to be split into four sub-objects in the slicer for accent colorization.  I found that Paramount Red ABS was somewhat translucent and darkened when a black back layer was applied over the accent. The STL contains an extra color change back layer to cover the red accent color.  I found the red really popped with a white or silver back layer.


## Assembly ##

Insert six heat set inserts into each of the FilterMainL and FilterMainR parts making sure the inserts are flush or below the plastic.
![](./images/Inserts.jpg?raw=true)

Add M3x8 screws to the four outermost inserts leaving about 3mm of the screw thread exposed.
![](./images/Screws.jpg?raw=true)

Take the perfectly good 5015 blowers and cut the leads to about 80mm.  Solder and heat shrink the blower leads to the 2P JST housings, keeping the red/black orientation matching the original leads.

Insert a soldered JST housing into each of the FilterMain parts, noting the orientation. The gap in the JST connector should face down.  Insert the connector at an angle, then press flat until it snaps into place. 
![](./images/Insert_JST.jpg?raw=true)

![](./images/JST_Orientation.jpg?raw=true)

Starting at a slight angle, slide a ConnClamp over each JST housing.  The ConnClamp should snap into place with some modest pressure.
![](./images/InsertRetainer1.jpg?raw=true)

Orient the 5015 blowers to line up with the exhaust phlenum and secure in place with BlowerHoldDowns and M3x8 screws.  Tuck in the excess blower wire.

![](./images/HoldDowns.jpg?raw=true)

Trial fit the FilterTop onto each FilterMain, slide into place and snug up the four retaining screws.  Verify that the FilterTop aligns and squares up with the FilterMain and forms a tight fit with the CarbonFilter cartridge. Depending on your print quality, lightly sand away any 3D print imperfections on the mating surfaces.  It doesn't have to be perfect.  

![](./images/AttachTop.jpg?raw=true)

Inspect the magnet pockets for 3D print irregularities and trial fit the magnets.   A piece of wax paper is a convenient separator between the magnets as they are glued in, allowing the cartridge to be pressed against the FilterMain/FilterTop assembly. Orient the magnet pairs so they attract, separated by the wax paper. When satisified with the fit add a drop of CA to glue the magnets into place.  
  
The RoboVac filter can be inserted with the extraction ribbon facing outwards or inwards.  If facing outwards, it doesn't sit as flat under the foam prefilter and obstructs a small amount of the filter surface.  My preference is to install inwards in which case a small Allen wrench can be inserted as shown to pry out the filter when it comes time for removal.

![](./images/InsertFilterTab.jpg?raw=true)

Add the foam prefilter that comes with with the RoboVac filters and snap the FilterScreen into place.  A  finger nail or small screwdriver can be inserted as shown to pry off the FilterScreen as needed when replacing the filters.

![](./images/InsertFilterScreen.jpg?raw=true)

I recommend testing each filter before it is installed in the printer. If a power supply is available, check the fan is drawing at least 80mA.  There are a lot of underpowered counterfeit fans in the supply chain that only draw a fraction of this power with drastically reduced airflow.

Check the fit of each FilterDoor by sliding them into the CarbonFilters.  They should just fit and snap into place when fully inserted. Remove any elephant foot or blobs as needed. Note there is a chamfer on the edge of each door that mates into the dovetail grove of the CarbonFilters so be sure to get the orientation correct. Slide the funnel into place as shown and fill each of the two chambers of each CarbonFilter with activated charcoal. Gently tap and jiggle the filter so the carbon settles.  If the chamber is not completely full, air will bypass over the top of the charcoal layer reducing the effectiveness of filter.  Insert the FilterDoor as each chamber is filled.

![](./images/PXL_20241231_004722283a.jpg?raw=true)

## Installation ##

The filters can be mounted so the exhaust is directed towards the front or back of the chamber according to personal preference.  I haven't seen any draft/warping issues with rear mounted filters with front facing exhausts as pictured.

Start by removing the HEPA filters, FilterScreens and the FilterTop of each filter by backing out the four M3 screws holding the FilterTop by a couple of turns.  Removing the FilterTop provides access to the two mounting holes.  Insert two half round T nuts into the 2020 channel and slide so the holes line up with holes in each FilterMain.  The Right and Left FilterMain have unused mounting holes blocked off. Insert the M3x8 screws with M3x9mm washers and secure the FilterMain where indicated below with the yellow arrows.  The [TPU Z belt covers](https://github.com/VoronManiac/Maniac-Chamber-Lighting/blob/main/STL/Common/DeckCornerRightRear.stl) shown are used in the  [Low Glare LED Maniac-Chamber-Lighting](https://github.com/VoronManiac/Maniac-Chamber-Lighting/tree/main) project and have channels for routing the power leads to the filters.  If you decide not to use these z-belt covers, plan out your wire routing for the filter power leads. 

![](./images/PXL_20241231_002415320a.jpg?raw=true)


Once satisfied with the position tighten the FilterMain into place.    Allow the CarbonFilter cartridge to snap to the FilterMain and FilterTop then lock the FilterTops into place by snugging the four retaining screws with an allen wrench as shown below.  Re-install the HEPA filters, foam prefilter, and FilterScreens.


![](./images/PXL_20241231_003405013.MPa.jpg?raw=true)



Wire routing with power leads connected to JST using the TPU z-belt cover from the LED project as shown below.

![](./images/PXL_20241231_003657176a.jpg?raw=true)


![](./images/PXL_20241231_003556793a.jpg?raw=true)

## Special Considerations ##
The filter Z height is constrained to 35mm max which is slightly below the print bed surface of a typical V2.4.  Check that your printer has the 35mm of clearance.  In some earlier V2.4 machines, the M3 SHCS that holds the X/Y endstop switch housing in place can be replaced with BHCS or the housing can be modified to completely recess the screws.  The clearance might also be a function of hot end length and z-home switch.<br>

## FW Setup ##
Add the following to `printer.cfg` so that the filters come on when the extruder or bed are above 90C.  The extra airflow across and under the bed helps heat the chamber a bit more quickly at the start of a print.<br>
```
 [heater_fan filter_fan]

  pin: PD12  #machine specific
  kick_start_time: 0.5
  heater: heater_bed, extruder
  heater_temp: 90.0
```


















