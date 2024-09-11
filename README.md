# V2.4-Aire #
Each Aire filter has a HEPA particle prefilter followed by an activated charcoal filter, and is targeted at Voron 2.4 250/300/350 printers. Ideally, a pair of filters is mounted on either side of the print bed.  The filter Z height is constrained to 35mm max which is slightly below the print bed surface of a typical V2.4.

![](./images/PXL_20240910_233532594a.jpg?raw=true)

The design is optimized for high air flow to increase the turnover rate of heated chamber air.  Aire uses inexpensive Eufy RoboVAC HEPA filters.  The Eufy HEPA filter sits above the 5015 blower, but sufficient space is provided between the two to prevent the blower from stalling.  The blower exhaust feeds the single piece activated carbon cartridge.  The cartridge attaches to the HEPA/blower section with magnets. Once loaded with charcoal, two small doors slide into place to close off the cartridge. 

As shown below, the airpath in the cartridge splits into two sections, passing through a 17mm wide layer of charcoal,  and then gets collected in the output plenums.  The split path and relatively thin width of charcoal reduce blower back pressure and helps increase airflow.  Each 95mm cartridge has similar charcoal capacitiy compared to NeverMore DuoV5.  The 95mm cartridge could be redesigned to further increase the charcoal volume by lengthening it, which incidentially would *decrease* the blower back pressure and increase airflow.

![](./images/AirFlow.jpg?raw=true)

The charcoal and Eufy air filters should probably be replaced after 16 to 20 kg of ABS/ASA, but this is dependent on many factors including the brand of ABS/ASA.  It is on the to-do list to measure particle counts and VOC levels.  The pic below shows a dirty filter after 4 months of usage compared to a fresh filter.




## BOM ##
| Qty        | Item           | Comment |
|:------------- |:------------- |:----- |
|2           | Eufy RoboVac Filter 110x48x10(mm)| https://www.amazon.com/gp/product/B07F5XK5WN/ref=ppx_yo_dt_b_search_asin_title  |
|2           |GDSTIME 5015 Turbo Dual BB 24V  | https://www.amazon.com/gp/product/B0B1V6JTB8/ref=ppx_yo_dt_b_search_asin_title  |
|1      | 2-Pin 2.5mm JST Male Pin Header | like https://www.digikey.com/en/products/detail/jst-sales-america-inc./B2B-XH-A/1651045 |
| 16      | M3x8 BHCS |  |
| 4 | M3 9mm washer |    |
| 12 |  M3 Heatset Insert | |
| 16 | N52 magnets 6mm dia x 3mm thick|| 
| bag | activated charcoal | |




