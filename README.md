# ML-Portfolio

This is a basic repo cataloging some notebooks from Gavin Leeper's recent projects.
None of this is production ready per se, but it takes advantage of Git's reliable rendering of Jupyter notebooks in the browser.

## ChordNamer

This is a research notebook for a Python script that was ultimately deployed [here](https://github.com/e7mac/chord_namer) as part of [ChordNamer](http://chordnamer.link/), a project I helped submit to [ISMIR 2024](https://ismir2024.ismir.net/). 

ChordNamer takes a MusicXML file (a universal sheet music format between score editors), and returns a MusicXML file with chord names calculated for each measure. It works on an arbitrary number of staves, so even orchestral scores will work. It accounts for some edge cases like passing tones, and descending bass lines. ChordNamer was accepted for presentation as a late breaking demo. Demo video can be found [here](https://drive.google.com/file/d/1SjkC2pUtKQcSYCUphnJ5BIyWA6kb_ChM/view?usp=sharing).

## Amtrak Project

I set out to make a model to predict arrival delays for Amtrak trains. I've been collaborating with [ASMAD](https://juckins.net/amtrak_status/archive/html/home.php), a homegrown database with some of the only reliable historical data on arrivals and departures. 

As you'll see in the notebook, most of the work so far has been data munging and feature engineering. With the existent data, I've only been able to get an R^2 of about 15% with xgboost so far. At some point, I'd like to add on weather data to see if that improves predictions. Short of building a robust model, a thorough analysis to simply identify bottle neck stations and trends would still probably provide value for Amtrak managers.
