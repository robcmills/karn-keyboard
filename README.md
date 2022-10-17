# karn-keyboard

Custom, low profile, split, ortholinear, non-staggered, wireless, 38 key keyboard

What makes the Karn unique are the 1.5u thumb arc keys, the 1.5u pinky reach keys, and the status LEDs.

![karn-right-assembled](/images/karn-right-assembled.jpg "karn-right-assembled")


### Thumb Arc Keys

I didn't like "tucking" my thumb under my palm, and most other keyboards I found in this "Ferris" family of split, minimal keyboards have thumb keys located "inside" of the homing fj keys' column. 

The Karn aligns the inner thumb key with the homing column. This feels comfortable to me, and provides a sense of "homing" to my thumbs as well. With the additional thumb keys splaying out inwards from there, in a more aggresive downward arc than the Ferris. This arc follows the natural arc of my thumb. I took photos and did measurements.

![ergo-reference-neutral-thumb-key](/images/ergo-reference-neutral-thumb-key.png "ergo-reference-neutral-thumb-key")

Also, the thumb keys are designed for vertical 1.5u keycaps. This is because I found 1u keycaps uncomfortable for my thumbs, as I typically make contact with the side of my thumb, which has more surface area making contact, and the sharp edge of 1u keycaps would dig into the center of the area of skin making contact. 

![thumb-key-edge-discomfort](/images/thumb-key-edge-discomfort.jpg "thumb-key-edge-discomfort")

Other keyboards are designed with maybe one or two larger thumb keys, but they are typically 2u, which means the added complexity of stabilizers, in addition to just feeling too big.


### Pinky Reach Keys

"Pinky reach" meaning the keys in the colmn "outside" of the pinky column. On a traditional keyboard this would correspond to the Escape, Tab, Caps-lock, and Shift keys on the left hand for example. The other keyboard designs I saw either had no pinky reach keys, or a full set of three or four. The Karn is designed very much in the "all keys within one key distance of home" style, as is common in the less than 40% category. However, although the pinky diagonal reaches technically still count as "one key distance", that reach felt too difficult to me. And so they are omitted, but having zero pinky reach keys, I found it difficult to fit Tab and Enter elsewhere. There were just too few keys at that point, and so I wanted to retain a single horizontal pinky reach key on each side. I use these for Tab, Enter, and hold for Hyper. 


### Status LEDs

The Karn is designed to be minimal, and easy to assemble. As such, I omitted LEDs for each key, but there are three LEDs positioned next to the microcontroller on only the right hand side. The purpose of these are as follows:

1. Current Layer
2. Caps-lock indicator
3. Battery level

I had considered an OLED screen, but that requires looking down at the keyboard and focusing on it in order to read what the current layer is. An LED can be seen out of the corner of your eye without breaking your gaze and focus away from the screen.


### Parts List

- key switches
https://mkultra.click/choc-switches
Kailh Low Profile Choc v1

- key caps
https://mkultra.click/mbk-choc-keycaps

- microcontroller
https://mkultra.click/nice-nano-v2/
(includes 301230 110mAh Battery with JST Connector) 

- microcontroller sockets and pins
https://mkultra.click/mill-max-micro-controller-sockets-and-pins/

- power switches
https://mkultra.click/alps-ssss811101/
https://tech.alpsalpine.com/e/products/detail/SSSS811101/

- diodes
https://www.digikey.com/en/products/detail/micro-commercial-co/1N4148X-TP/789328
PART: 1N4148XTPMSCT-ND
MFG : MICRO COMMERCIAL CO (VA) / 1N4148X-TP
DESC: DIODE GEN PURP 75V 150MA SOD523
UNIT PRICE: $0.173

- leds
https://www.digikey.com/en/products/detail/adafruit-industries-llc/2686/5804107
PART: 1528-1541-ND
MFG : ADAFRUIT INDUSTRIES LLC / 2686
DESC: ADDRESS LED DISC SERIAL RGB 10PK
UNIT PRICE: $4.95 (for quantity 10)

- battery connectors
https://www.digikey.com/en/products/detail/jst-sales-america-inc/S2B-PH-K-S-LF-SN/926626
PART: 455-1719-ND
MFG : JST SALES AMERICA INC / S2B-PH-K-S(LF)(SN)
DESC: CONN HEADER R/A 2POS 2MM
UNIT PRICE: $0.134

- reset switches
https://www.digikey.com/en/products/detail/e-switch/TL3313AF250QG/4029401
PART: EG6065CT-ND
MFG : E-SWITCH (VA) / TL3313AF250QG
DESC: SWITCH TACTILE SPST-NO 0.05A 12V
UNIT PRICE: $0.431

- bottom
Non Slip Anti Skid Pads Self-Stick 2 Pieces Black Rubber 4x6 inch
https://www.amazon.com/dp/B08HN5R9Y3

- pcb
https://www.pcbway.com/


### Firmware

https://github.com/robcmills/karn-keyboard-firmware

