pantaliQa-core
==============

Description
pantaliQa-core is a collection of puredata patches for video manipulation in realtime. 
It has been developed with the aim to prototype vjing kind of application in puredata+Gem. 
It is based on puredata vanilla, some library packaged under debian/ubuntu multimedia repository and it was designed having in mind pdp external but using the Gem (opengl) library.
Design
PantaliQa-core has a collection of objects ideally categorized under 4 different type: source, process, effect, output.
By connecting a source and an output object you are ready to go fullscreen.
The idea behind every object is to do more with less. The library make all the geometry calculation Gem need for you.
Every object has one inlet for the render chain (not the cases for source objects that starts the chain) and one inlet for message control. By a set of registered messages for every object you can control all the properties of the object. This properties are accessible also through a standard pattern message osc-style system: 
/q/name_of_the_object/name_of_the_istance/property
With that system is easy to communicate with every object in the patch and also to make communicate them with external applications.
Every property is normalized between 0 and 1. 

GUI
===
PantaliQa-core is intended to be imported in other patch systems. One of the connected projects is to build a gui system (using pd-l2ork or wx-python) which will be in charge to get get midi, OSC, keyboard signals and assign them to the objects dynamically. For this reason pantaliQa-core doesn't support any of this library. 

INSTRUCTION
===========
Check the wiki: https://github.com/pantaliQa/pantaliQa-core/wiki 

THE NAME
========
This project came from an older one called Qeve and presented during III international Puredata conference in Sao Paulo: this the reason for "Q" letter Brand of the project kind of.
Pantalica is the oldest necropolis in Europe, situated in Sicily, my island of origin. The first time I design this new project I was there and the name is a celebration of that moment.






