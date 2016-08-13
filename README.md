#### My universal Brouter profile template for bike profiles

* This is a development version of Bicycle profile template, that may be a head of the released [Bicycle profiles](https://github.com/poutnikl/Brouter-profiles/raw/master/BR-Bike-Profiles.zip). 
* See more at [Brouter-profiles](https://github.com/poutnikl/Brouter-profiles).

* You can derive respective development versions of the profiles from this latest [Template file](https://raw.githubusercontent.com/poutnikl/Trekking-Poutnik/master/Trekking-Poutnik.brf) by 2 ways. 

    * 1/ Use modification table below ( for now not covering all profiles ). While saving, do not forget the .brf extension.
    * 2/ Use this [Windows batchfile sedbatch.bat](https://raw.githubusercontent.com/poutnikl/Brouter-profiles/master/sedbatch.bat). 
        * Check its prerequisities inside the batch code ( presence and provided location of sed.exe, wget.exe and (optionally) 7z.exe utilities.
        * Run the batch with "bike" parameter as "sedbatch bike" from the Windows command line.



|Profile name/code     |What to change / was changed    |Comment                                                   |
|----------------------|--------------------------------|----------------------------------------------------------|
|Trekking-Dry          |Nothing                         |Template default content is identical to this profile     |
|-Wet                  |assign iswet 1                  |To be used in wet weather, penalizes potentially          |
|                      |                                |penalizing wet/potentially muddy conditions               |
|-FCR-                 |assign cycleroutes_pref 0.6     |Stronger preference of cycleroutes      |   
|(FollowCycleRoute)    |                                |works differently to standard Trekking.brf                |
|-ICR-                 |assign cycleroutes_pref 0.0     |No preference for cycleroutes. Values >0.0 up to 1.0      |
|                      |                                |progressively prefer long distance icn,ncn                |
|                      |                                |and similarly penalize  non cycleroutes                   |
|                      |                                |Effects are stronger for not optimal ways                 |
|-SameCR               |assign routelevel 4             |Preference of local/regional routes is as strong as       |
|                      |                                |for long distance routes ( normally about the half )      |
|Trekking-MTB-light    |assign MTB_factor 0.2           |See [Trekking-MTB-Profiles-legend](https://github.com/poutnikl/Brouter-profiles/wiki/Trekking-MTB-Profiles---legend)|
|Trekking-MTB-medium   |assign MTB_factor 0.5           |  |
|Trekking-MTB-strong   |assign MTB_factor 1.0           |                                                          |
|Trekking-Fast         |assign MTB_factor -0.5          | "Anti-MTB"                                               |
|MTB-light             |assign MTB_factor 1.0           | [See Locus forum post](http://forum.locusmap.eu/index.php?topic=4883.msg41428#msg41428)                                                      |
|                      |                                |See also [MTB_factor-and-smallpaved_factor](https://github.com/poutnikl/Brouter-profiles/wiki/MTB_factor-and-smallpaved_factor)|
|                      |assign smallpaved_factor -0.3   |                                                          |
|MTB                   |assign MTB_factor 2.0           |                                                          |
|                      |assign smallpaved_factor -0.5   |                                                          |
|Trekking-Valley       |assign hills 4                  | Strongly penalizes ascends/descends. Prefers large       |
|                      |                                | percentage of flat-like route along the valleys          |
|SmallRoads            |assign MTB_factor -1.7          | Prefers way classes approx since terciary roads          |
|                      |assign smallpaved_factor 2.0    | to  paved tracks                                         |


* See also 
    * [Brouter-profiles](https://github.com/poutnikl/Brouter-profiles) and
    * [Brouter profiles wiki pages](https://github.com/poutnikl/Brouter-profiles/wiki)
