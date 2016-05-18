#### My universal Brouter profile template for bike profiles

This is a development version. You can easily derive up-to-date versions of my [bicycle profiles](https://github.com/poutnikl/Brouter-profiles/wiki/Bicycle-Trekking-profiles) from this latest [Template file](https://raw.githubusercontent.com/poutnikl/Trekking-Poutnik/master/Trekking-Poutnik.brf). 
While saving, do not forget the .brf extension.

|Profile name          |What to change                  |Comment                                              |
|----------------------|--------------------------------|-----------------------------------------------------|
|Trekking-Dry          |Nothing                         |Template default content is identical to this profile|
|Trekking-Wet          |assign iswet 1                  |To be used in wet/potentially muddy conditions       |
|                      |                                |It can be combined with MTB_factor as wet variants   |
|Trekking-ICR          |assign cycleroutes_pref 0.0     |No preference for cycleroutes. Values >0.0 up to 1.0 |
|                      |                                |progressively prefer long distance icn,ncn           |
|                      |                                |and similarly penalize  non cycleroutes              |
|                      |assign routelevel 1..4          |Defined what is considered long distance route yet   |
|                      |                                |1-icn only, 2 +ncn(default), 3 +rcn, 4 all           |
|Trekking-MTB-light    |assign MTB_factor 0.2           |See [Trekking-MTB-Profiles legend](https://github.com/poutnikl/Brouter-profiles/wiki/Trekking-MTB-Profiles---legend)                                                     |
|Trekking-MTB-medium   |assign MTB_factor 0.5           |                                                     |
|Trekking-MTB-strong   |assign MTB_factor 1.0           |                                                     |
|Trekking-Fast         |assign MTB_factor -0.5          | "Anti-MTB"                                          |
|MTB-light             |assign MTB_factor 1.0           | [See Locus forum post](http://forum.locusmap.eu/index.php?topic=4883.msg41428#msg41428)                                                 |
|                      |assign smallpaved_factor -0.3   |                                                     |
|MTB                   |assign MTB_factor 2.0           |                                                     |
|                      |assign smallpaved_factor -0.5   |                                                     |
|Trekking-Valley       |assign hills 4                  | Strongly penalizes ascends/descends. Prefers large  |
|                      |                                | percentage of flat-like route along the valleys     |
|SmallRoads            |assign MTB_factor -1.7          | Prefers way classes approx since terciary roads     |
|                      |assign smallpaved_factor 2.0    | to  paved tracks                                    |


[Visit also my Brouter profiles wiki pages](https://github.com/poutnikl/Brouter-profiles/wiki)
