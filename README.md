pantaliQa-core
==============

pantaliQa-core is a collection of puredata patches for video manipulation in realtime. 
It has been developed with the aim to prototype vjing kind of application in puredata+Gem. 
It is based on puredata vanilla, some library packaged under debian/ubuntu multimedia repository and it was designed having in mind pdp external but using the Gem (opengl) library.
Design
PantaliQa-core has a collection of objects ideally categorized under 4 different type: source, process, effect, output.
By connecting a source and an output object you are ready to go fullscreen.
The idea behind every object is to do more with less. The library does all the geometry calculation Gem needs for you.
Every object has one inlet for the render chain (not the cases for source objects that start the chain) and one inlet for message control. By a set of registered messages for every object you can control all the properties of the object. This properties are accessible also through a standard pattern message osc-style system: 
/q/name_of_the_object/name_of_the_istance/property
With that system it's easy to communicate with every object in the patch and also to make them communicate with external applications.
Every property is normalized between 0 and 1. 

GUI
===
PantaliQa-core is part of PantaliQa project and is intended to be imported in other patch systems. One of the connected projects is a gui system (using pd-l2ork or wx-python) which will be in charge of getting midi, OSC, keyboard signals and assign them to the objects dynamically. For this reason pantaliQa-core doesn't support any of this library. 

INSTRUCTIONS
===========
Check the wiki: https://github.com/pantaliQa/pantaliQa-core/wiki 

NAME
========
This project came from an older one called Qeve and presented during III international Puredata conference in Sao Paulo: this the reason for "Q" letter Brand of the project kind of.
Pantalica is the oldest necropolis in Europe, situated in Sicily, my island of origin. The first time I design this new project I was there and the name is a celebration of that moment.


THANKS
======

PantaliQa-core is develop by my, Luca_at_estereotips_dot_net in my free time.
It has been possible thanks to the support, testing effort and use of Luca Franceschini.
None of this would be possible without the great puredata community, the developpers and the users both.
Expecially thanks to the devs of Extended Toolkit from which I copied some abstraction.







