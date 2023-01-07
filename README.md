# karn-keyboard

Split, ortholinear, non-staggered, 38 key keyboard.

What makes the Karn unique are the 1.5u thumb arc and pinky reach keys.

![karn-right-assembled](/images/karn-right-assembled.jpg "karn-right-assembled")

![karn-complete](/images/karn-complete.jpg "karn-complete")

### Thumb Arc Keys

I didn't like "tucking" my thumb under my palm, and most other keyboards I found in this "Ferris" family of split, minimal keyboards have thumb keys located "inside" of the homing fj keys' column. 

The Karn aligns the inner thumb key with the homing column. This feels comfortable to me, and provides a sense of "homing" to my thumbs as well. With the additional thumb keys splaying out inwards from there, in a more aggresive downward arc than the Ferris. This arc follows the natural arc of my thumb. I took photos and did measurements.

![ergo-reference-neutral-thumb-key](/images/ergo-reference-neutral-thumb-key.png "ergo-reference-neutral-thumb-key")

Also, the thumb keys are designed for vertical 1.5u keycaps. This is because I found 1u keycaps uncomfortable for my thumbs, as I typically make contact with the side of my thumb, which has more surface area making contact, and the sharp edge of 1u keycaps would dig into the center of the area of skin making contact. 

![thumb-key-edge-discomfort](/images/thumb-key-edge-discomfort.jpg "thumb-key-edge-discomfort")

Other keyboards are designed with maybe one or two larger thumb keys, but they are typically 2u, which means the added complexity of stabilizers, in addition to just feeling too big.


### Pinky Reach Keys

"Pinky reach" meaning the keys in the colmn "outside" of the pinky column. On a traditional keyboard this would correspond to the Escape, Tab, Caps-lock, and Shift keys on the left hand for example. The other keyboard designs I saw either had no pinky reach keys, or a full set of three or four. The Karn is designed very much in the "all keys within one key distance of home" style, as is common in the less than 40% category. However, although the pinky diagonal reaches technically still count as "one key distance", that reach felt too difficult to me. And so they are omitted, but having zero pinky reach keys, I found it difficult to fit Tab and Enter elsewhere. There were just too few keys at that point, and so I wanted to retain a single horizontal pinky reach key on each side. I use these for Tab (left), Enter (right), and hold for Hyper. 


### Versions

There are actually two versions in this repo: 

### Karn-1

The original version is designed to be wireless. It is built around a standard 24 pin microcontroller with bluetooth support. I used the Nice-Nano-v2. With only 24 pins and 38 keys, this necessitated a matrix key layout, with diodes. Additionally, it adds an on/off switch, reset switch, and battery connector. This makes assembly much more complicated. Especially the diodes, which are super tiny, and very difficult to hot-air solder onto the tiny pads. This is not for beginners.

Also, the original karn pcb is split across two different designs, one for the left and another for the right. This doubles manufactoring costs, since you have to order the pcbs for both sides. I was learning.

### Karn-2

The karn-2 seeks to improve on the original with a host of simplifications. It is built around a 40 pin microcontroller so that there is no need for a key matrix, and hence no diodes. Furthermore, the microcontroller I found has a reset switch built onto the board, so no extra parts and hot-air soldering required. The microcontroller does not support Bluetooth, but this means no battery connector and no on/off switch. This greatly simplifies the design and assembly, and reduces the number of parts required and thus the cost.

And lastly, the karn-2 PCB is designed to be reversible, so you only need to order it once, and you can use it for both left and right. 

![karn-2-pcb](/images/karn-2-pcb.png "karn-2-pcb")


### Parts List

- key switches
https://mkultra.click/choc-switches
Kailh Low Profile Choc v1

- key caps
https://mkultra.click/mbk-choc-keycaps

- microcontroller (karn-1)
https://mkultra.click/nice-nano-v2/
(includes 301230 110mAh Battery with JST Connector) 

- microcontroller (karn-2)
https://www.digikey.com/en/products/detail/dfrobot/DFR0864/14824968
DFRobot Blackpill development board

- microcontroller sockets and pins (karn-1)
https://mkultra.click/mill-max-micro-controller-sockets-and-pins/

- microcontroller sockets and pins (karn-2)
https://www.digikey.com/en/products/detail/mill-max-manufacturing-corp/315-43-120-41-003000/4455248
Mill-max 315-43-120-41-003000 sockets
https://www.digikey.com/en/products/detail/mill-max-manufacturing-corp/3320-1-00-15-00-00-03-0/4147393
Mill-max 3320-1-00-15-00-00-03-0 pins

- trrs jack
https://mkultra.click/pj-320a-3-5mm-trrs-jack/

- power switches (karn-1)
https://mkultra.click/alps-ssss811101/
https://tech.alpsalpine.com/e/products/detail/SSSS811101/

- diodes (karn-1)
https://www.digikey.com/en/products/detail/micro-commercial-co/1N4148X-TP/789328
PART: 1N4148XTPMSCT-ND
MFG : MICRO COMMERCIAL CO (VA) / 1N4148X-TP
DESC: DIODE GEN PURP 75V 150MA SOD523
UNIT PRICE: $0.173

- leds (karn-1)
https://www.digikey.com/en/products/detail/adafruit-industries-llc/2686/5804107
PART: 1528-1541-ND
MFG : ADAFRUIT INDUSTRIES LLC / 2686
DESC: ADDRESS LED DISC SERIAL RGB 10PK
UNIT PRICE: $4.95 (for quantity 10)

- battery connectors (karn-1)
https://www.digikey.com/en/products/detail/jst-sales-america-inc/S2B-PH-K-S-LF-SN/926626
PART: 455-1719-ND
MFG : JST SALES AMERICA INC / S2B-PH-K-S(LF)(SN)
DESC: CONN HEADER R/A 2POS 2MM
UNIT PRICE: $0.134

- reset switches (karn-1)
https://www.digikey.com/en/products/detail/e-switch/TL3313AF250QG/4029401
PART: EG6065CT-ND
MFG : E-SWITCH (VA) / TL3313AF250QG
DESC: SWITCH TACTILE SPST-NO 0.05A 12V
UNIT PRICE: $0.431

- feet
Self-Adhesive Clear Rubber Feet Tiny Bumpons (6x2mm)
https://www.amazon.com/dp/B06XCNM69B

- pcb
https://www.pcbway.com/


### Firmware

https://github.com/robcmills/karn-keyboard-firmware


### Inspiration

#### Thumb Block Style

- Maltron https://en.wikipedia.org/wiki/Maltron

![maltron](/images/maltron.jpg "maltron")

- Kinesis Advantage https://kinesis-ergo.com/shop/advantage2/

![kinesis-advantage](/images/kinesis-advantage.jpg "kinesis-advantage")

- Ergodox EZ https://ergodox-ez.com/

![ergodox-ez](/images/ergodox-ez.webp "ergodox-ez")


#### Thumb Arc Style

- NEC PWP http://xahlee.info/kbd/nec_pc-8801_keyboard.html

![nec](/images/nec-pc-8801-k1.jpg "nec")

- Kyria https://blog.splitkb.com/blog/introducing-the-kyria

![kyria](/images/kyria.jpg "kyria")

- Corne https://github.com/foostan/crkbd

![corne](/images/corne.jpg "corne")
