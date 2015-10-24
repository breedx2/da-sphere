# da-sphere
This is a project to create a status light and general fun hack project.

![Alt text](/da-sphere.jpg?raw=true "DA Team Status Sphere")

Currently there are 60 individually addressable LEDs that can produce the entire spectrum. The unit is connected to WiFi (FSGuest) and is relayed HTTP Posts to the Particle.io API. It can run without wall power for a while, but will eventually run out of batteries(~48 hours). While plugged in it will stay charged and ready to go.
![Alt text](/photon-neopixel-unit.jpg?raw=true "Photon and Neopixel Ring")



##How to call functions on the Particle.io API

HTTP Post Format:

     curl https://api.particle.io/v1/devices/<Particle.io-Photon-ID>/<Function> -d access_token=<Particle.io-API-Key>

###Available Functions

####color

HTTP Post Format:

     curl https://api.particle.io/v1/devices/<Particle.io-Photon-ID>/color -d access_token=<Particle.io-API-Key> -d arg=<COLOR>

Available Colors
     off
     black
     white
     red
     blue
     green
     yellow
     purple
     cyan
     orange
     pink
     rainbow
