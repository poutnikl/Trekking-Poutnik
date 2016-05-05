#### Trekking-Poutnik Brouter profile template for bikes

This is a development version. You can easily derive up-to-date versions of my [bicycle profiles](https://github.com/poutnikl/Brouter-profiles/wiki/Bicycle-Trekking-profiles) based on the latest [Template file](https://raw.githubusercontent.com/poutnikl/Trekking-Poutnik/master/Trekking-Poutnik.brf). 
While saving, do not forget the .brf extension.

|Profile name          |What to change                  |Comment                                              |
|----------------------|--------------------------------|-----------------------------------------------------|
|Trekking-Dry          |Nothing                         |Template default content is identical to this profile|
|Trekking-Dry          |assign iswet 1                  |To be used in wet/potentially muddy conditions       |
|                      |                                |It can be combined with MTB_factor                   |
|Trekking-MTB-light    |assign MTB_factor 0.2           |                                                     |
|Trekking-MTB-medium   |assign MTB_factor 0.5           |                                                     |
|Trekking-MTB-strong   |assign MTB_factor 1.0           |                                                     |
|Trekking-Fast         |assign MTB_factor -0.5          | "Anti-MTB"                                          |
|MTB-light             |assign MTB_factor 1.0           |  1)                                                 |
|                      |assign smallpaved_factor -0.3   |                                                     |
|MTB                   |assign MTB_factor 2.0           |                                                     |
|                      |assign smallpaved_factor -0.5   |                                                     |

1) - [See Locus forum post](http://forum.locusmap.eu/index.php?topic=4883.msg41428#msg41428)
