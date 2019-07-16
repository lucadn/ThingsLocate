# ThingsLocate
A ThingSpeak-based platform for indoor positioning of IoT devices using WiFi fingerprinting

The platform includes two main components:

a) Matlab code to be imported in a ThingSpeak Matlab analysis app, that reacts to WiFi fingerprinting data uploaded on a set of input ThingSpeak channels (RSSI channels), determines the position of the device that uploaded the data, and returns the position estimation on an output ThingSpeak Channel (Locate channel). Several different algorithms and metrics can be selected in the Locate App.

b) client-side code for the following devices:
- Raspberry Pi using Raspbian / Linux machines (Python script)
- Mac Os (Python script)
- Android (native app)
Irrespectively of the device, the code offers the following features: 
- Automatic averaging of multiple WiFi scans with customizable number of scans, to counteract channel variability
- Automatic sorting of averaged measurements, in order to minimize the impact of dropping measurements when too many APs are detected
- Local file storage of measurements, allowing for easy collection of Test Points/Reference Points in known locations

(c) Luca De Nardis, 2018
When using this platform in scientific publications, please refer to the following work:

L. De Nardis, G. Caso, M. G. Di Benedetto, "ThingsLocate: a ThingSpeak-based indoor
positioning platform for academic research on location-aware Internet of Things," to appear in MDPI Techologies, Special  Issue "Technology Advances on IoT Learning and Teaching, "2019.
