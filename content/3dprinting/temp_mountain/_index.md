---
title: 'Temperature Mountain'
date: 2024-09-14T00:00:00
weight: 1
menu_page: true
show_date: true
---

A 3D model of the global temperature of Earth over the last 100 years.
<!--more-->
## Description

Inspired by the [Temperature Spiral](https://ed-hawkins.github.io/climate-visuals/spirals.html) by [Ed Hawkins](https://github.com/ed-hawkins)[^1], this model shows the global mean surface temperature of Earth for the last 100 years (1924 to 2023).

<img src="/images/temp_mountain_2023/photo.jpg" alt="Photo of the Temperature Mountain" width="434"/>

Temperatures are taken from the [HadCRUT v5.0.2.0](https://www.metoffice.gov.uk/hadobs/hadcrut5/data/versions/HadCRUT.5.0.2.0_release_notes.html) published jointly by the UK Met Office Hadley Centre and the Climatic Research Unit at the University of East Anglia. This dataset contains anomalies from the 1961-1990 reference period of global temperatures, so it shows the progression of temperatures through the century but not absolute temperature values. The temperatures are presented as a complete spiral from January 1924 at the outer edge to December 2023 in the middle. The spiral is 12-sided, with each point representing a single month. The height of each point is scaled evenly between the lowest temperature during the period (which will be level with the base) and the highest temperature (the highest point of the mountain).

## Notes For Printing
This is quite a difficult model to print, with a very large number of retractions if printing on an FDM printer. (A resin printer would probably be better, but I haven't got one to test with.) This means that you need good retraction performance to get a clean result (which I clearly didn't!), and the print will take a significant amount of time (multiple days). To mitigate the time issue I have provided the model as either a single complete STL file, or multiple parts that can be glued together.

If printing multiple parts, it's best to push the 'mountain' parts together first to ensure they are all level before attaching the base. The tolerances for this are very tight, so you may need to set horizontal offset to a negative number in your slicer to give a little extra room.

The final print is very delicate, especially at the top. Using a stronger material than PLA may reduce the chances of knocking bits off by accident.

## Files and Code

The STL files for the Temperature Mountain are generated using Python and OpenSCAD. The scripts can be found on the [GitHub page](https://github.com/squaregoldfish/Climate3D).

### Single File
[all-in-one.stl (336 Kb)](/images/temp_mountain_2023/all-in-one.stl)

![OpenSCAD render of the all-in-one STL file](/images/temp_mountain_2023/all-in-one.png)


### Multiple Files
[temp_mountain_parts.zip (120 Kb)](/images/temp_mountain_2023/temp_mountain_parts.zip)

![OpenSCAD render of the separate parts](/images/temp_mountain_2023/parts.png)

## Licence
Temperature Mountain is licensed under [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/)


[^1]: Idea used with permission
