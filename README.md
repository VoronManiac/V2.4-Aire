# V2.4-Aire #
Each Aire filter has a HEPA particle prefilter followed by an activated charcoal filter, and is targeted at Voron 2.4 250/300/350 printers. Ideally, a pair of filters is mounted on either side of the print bed.  The filter Z height is constrained to 35mm max which is slightly below the print bed surface of a typical V2.4.

![](./images/PXL_20240910_233532594a.jpg?raw=true)

The design is optimized for high air flow to increase the turnover rate of heated chamber air.  Aire uses inexpensive Eufy RoboVAC HEPA filters.  The Eufy HEPA filter sits above the 5015 blower, but sufficient space is provided between the two to prevent the blower from stalling.  The blower exhaust feeds the single piece activated carbon cartridge.  The cartridge attaches to the HEPA/blower section with magnets. Once loaded with charcoal, two small doors slide into place to close off the cartridge. 

As shown below, the airpath in the cartridge splits into two sections, passing through a 17mm wide layer of charcoal,  and then gets collected in the output plenums.  The split path and relatively thin width of charcoal reduce blower back pressure and helps increase airflow.  Each 95mm cartridge has similar charcoal capacitiy compared to NeverMore DuoV5.  The 95mm cartridge could be redesigned to further increase the charcoal volume by lengthening it, which incidentially would *decrease* the blower back pressure and increase airflow.

![](./images/AirFlow.jpg?raw=true)

It is difficult to say how frequently the HEPA filter and charcoal need to be replaced without some direct particle and VOC measurements, but the pic below shows a dirty filter after 4 months of usage compared to a fresh filter. With the Zyltech ABS filament I have been running, the charcoal should last for many weeks of continuous printing.

![](./images/PXL_20240912_020730545b.jpg?raw=true)




## BOM ##
| Qty        | Item           | Comment |
|:------------- |:------------- |:----- |
|2           | Eufy RoboVac Filter 110x48x10(mm)| https://www.amazon.com/gp/product/B07F5XK5WN/ref=ppx_yo_dt_b_search_asin_title  |
|2           |GDSTIME 5015 Turbo Dual BB 24V  | https://www.amazon.com/gp/product/B0B1V6JTB8/ref=ppx_yo_dt_b_search_asin_title  |
|2      | 2-Pin 2.5mm JST Male Pin Header | like https://www.digikey.com/en/products/detail/jst-sales-america-inc./B2B-XH-A/1651045 |
| 16  | M3x8 BHCS |  |
|4|M3 Half Round Nuts|https://www.amazon.com/gp/product/B08YNFGYNH/ref=ppx_yo_dt_b_search_asin_title|
| 4 | M3 9mm washer |    |
| 12 |  M3xD5.0xL4.0 Heatset Insert | |
| 16 | N52 magnets 6mm dia x 3mm thick| | 
| 2  | 10mm 1.5mm Dia heat shrink tubing| |
| bag | activated charcoal | |

## Assembly ##

Insert six heat set inserts into each of the FilterMainL and FilterMainR parts making sure the inserts are flush or below the plastic.
![](./images/Inserts.jpg?raw=true)

Add M3x8 screws to the four outermost inserts leaving about 3mm of the screw thread exposed.
![](./images/Screws.jpg?raw=true)

Take the perfectly good 5015 blowers and cut the leads to about 80mm.  Solder and heat shrink the blower leads to the 2P JST housings keeping the red/black orientation matching the original lead.

Insert a soldered JST housing into each the FilterMain parts, noting the oriention of the JST housing. Insert at an angle, then press flat until it snaps into place. 
![](./images/Insert_JST.jpg?raw=true)

![](./images/JST_Orientation.jpg?raw=true)

Starting at a slight angle, slide a ConnClamp over each JST housing.  The ConnClamp should snap into place with some modest pressure.
![](./images/InsertRetainer1.jpg?raw=true)

Orient the 5015 blowers to line up with the exhaust phlenum and secure in place with BlowerHoldDowns and M3x8 screws.  Tuck in the excess blower wire.

![](./images/HoldDowns.jpg?raw=true)

Trial fit the FilterTop onto each FilterMain, slide into place and snug up the four retaining screws.  Inspect that the FilterTop aligns and squares up with the FilterMain and forms a tight fit with the CarbonFilter cartridge. Depending on your print quality, lightly sand away any 3D print imperfections on the mating surfaces.  Doesn't have to be perfect.  

![](./images/AttachTop.jpg?raw=true)

Inspect the magnet pockets for 3d print irregularities and trial fit the magnets.   A piece of wax paper is a convenient separator between the magnets as they are glued in, allowing the cartridge to be pressed against the FilterMain/FilterTop assembly. Orient the magnet pairs so they attract, separated by the wax paper. When satisified with the fit CA into place.  
  
The RoboVac filter can be inserted with the extraction ribbon facing outwards or inwards.  If facing outwards, it doeesn't sit as flat under the foam prefilter and obstructs a small amount of the filter surface.  My preferences is to install inwards in which case a small allen wrench can be inserted as shown to pry out the filter when it comes time for removal.

![](./images/InsertFilterTab.jpg?raw=true)

Add the foam prefilter that comes with with the RoboVac filters and snap the FilterScreen into place.  A  finger nail or small screwdriver can be inserted as shown to pry off the FilterScreen as needed when replacing the filters.

![](./images/InsertFilterScreen.jpg?raw=true)

I recommend testing each filter before it is installed in the printer.  Ideally if a power supply is available check the fan is drawing at least 80mA.  There are a lot of underpowered counterfeit fans in the supply chain that only draw a fraction of this power with drastically reduced airflow.

Check the fit of each FilterDoor by sliding them into the CarbonFilters.  They should just fit and snap into place when fully inserted. Remove any elephant foot or blobs as needed. Note there is a chamfer on the edge of each door that mates into the dovetail grove of the CarbonFilters so besure to get the orientation correct. Slide the funnel into place as shown and fill each of the two chambers of each CarbonFilter with activated charcoal. Gently tap and jiggle the filter so the carbon settles.  If the chamber is not completely full, air will bypass over the top of the charcoal layer reducing the effectiveness of filter.  Insert the FilterDoor as each chamber is filled.

![](./images/PXL_20241231_004722283a.jpg?raw=true)

## Installation ##

The filters can be mounted so the exhaust is directed towards the front or back of the chamber according to personal preference.  I haven't seen any issues with front facing exhausts when the filters are mounted towards the back of the chamber.

Start by removing the HEPA filters, FilterScreens and the FilterTop of each filter by backing out the four M3 screws holding the FilterTop by a couple of turns.  Removing the FilterTop provides access to the two mounting holes.  Insert two half round nuts into the 2020 channel and slide so the holes line up with holes in each FilterMain.  The Right and Left FilterMain have alternate unused mounting holes blocked off. Insert The M3x8 screws with M3x9mm washers and secure the FilterMain where indictated below with the yellow arrows.  The TPU Z belt covers shown are used in the Low Glare LED project and have channels for routing the power leads to the filters.  If you decide not to use these z-belt covers, plan out your wire routing for the filter power leads.

![](./images/PXL_20241231_002415320a.jpg?raw=true)


Once satified with the position tighten the FilterMain into place.    Allow the CarbonFilter cartridge to snap to the FilterMain and FilterTop then lock the FilterTops into place by snugging the four retaining screws with an allen wrench as shown below


![](./images/PXL_20241231_003405013.MPa.jpg?raw=true)

![](./imagesPXL_20241231_003556793a.jpg?raw=true)

![](./images/PXL_20241231_003657176a.jpg?raw=true)














