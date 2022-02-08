# MyoKey-EMG
sEMG data for MyoKey Experiments 

## Project overview

![interface](https://user-images.githubusercontent.com/32867191/151349677-b655ae26-1fa4-4413-a595-dc07f0f9c5b8.jpg)

MyoKey (aka MyoBoard) is a virtual keyboard for XR headsets. 
It takes into consideration textual input in the context of occupied hands (cylindrical and tripod grasp) as well as freehand.
sEMG signal from Myo Band on a user's forearm is used to decode subtle input gestures.  

## Dataset description

_data_ directory contains files named according to the following convention:

_**{participant} _ {year} _ {grasp} _ {gesture}**_

where:

_participant_ is in **{p0 .. p6}**,

_year_ is in **{2020, 2021}**,

_grasp_ is in **{freehand, cylindrical, tripod}**

_gesture_ is in **{idle, topRow, midRow, botRow, suggestion}**

Each file is a serialized array of 30 seconds long sEMG record captured on MyoBand at 200 Hz. 

For the graphical description please refer to the figure below. 

![Capture](https://user-images.githubusercontent.com/32867191/151349886-f2942f1e-f5f0-44a6-b12d-0307b6ddbc8a.PNG)
