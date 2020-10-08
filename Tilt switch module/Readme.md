![](p5.png)

![](p6.PNG)

## Descripcion

The tilt switch module known as KY 0 20. This is a module itself. So
let's get started. Today's video is brought to you by all our gv s and
an online store where you can find shirts, jeans and cool accessories
that fit your needs. All the products are made in Italy, they can be
shipped worldwide, so don't waste your time start looking fancy
today with their stock. For more information, go to RGV SM sharp
dot net or check it out at the link on the video description. This
module has integrated on board, a tilt switch, and one resistor, the
resistor using this module it's on and the main reason for using the
resistor is to limit currency collating inside the module.

In other words to prevent current from burning our modal. Now, I
will show how these components are connected together. There we
have the sensor itself, and of course, the resistor r1. On the right, you
can see how the piece of the module are connected on this board. So
we have inlet the flow of the voltage we have in black, the flow of
the ground, and of course, we have in game the flow of the signal.
This sensor has inside a metal egg bowl that opens or closes the
sacred step. panting.
The angle of the tilt the sensor it's normally have, but to under
sensor, it's tilted in that way that the ball shorts to conduct the sensor
turns on. Even that the sensor detects changes when it's tilted, it is
actually very basic and cannot measure the angle of the tilt. Let's talk
about the pins. The pins in this module

![](p7.PNG)

are three, we have the ground pin with a minus sign, the voltage
being is in the middle. And of course we have the pin of the signal
with the S sign. So let's talk about the signal. This module gives a


digital signal so we can connect the pins of the signal with any
digital ports of different microcontroller boards, like Arduino or
Raspberry Pi.


PIC1 | PIC2 |
------------ | -------------|
![](p8.PNG) | ![](p9.PNG)


## EXAMPLE SENSOR CODE:

int tiltPin = 2; // pin number for tilt switch signal

int ledPin = 13; // pin number of LED

int tiltState = 0; // variable for reading the tilt switch status

void setup() {

pinMode(ledPin, OUTPUT); // set the LED pin as output

pinMode(tiltPin, INPUT); // set the tilt switch pin as input



}

void loop(){

// get the tilt switch state

tiltState = digitalRead(tiltPin);

// check if tilt switch is tilted.

if (tiltState == HIGH) {

digitalWrite(ledPin, HIGH);

}

else {

digitalWrite(ledPin, LOW);




