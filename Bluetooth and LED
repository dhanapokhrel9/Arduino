String a; // to store date coming from app

int livingRoom = 12;// add the pin number that you want to control.

int basement = 11;// add the pin number that you want to control.

int bedRoom = 10;// add the pin number that you want to control.

void setup()

{

Serial.begin(9600);  // 9600 baud rate for serial monitor

// since we are turning on/off we need to output the pins
pinMode(livingRoom,OUTPUT);
pinMode(basement,OUTPUT);
pinMode(bedRoom,OUTPUT);

}

void loop() {

while(Serial.available()){  // until the date is availabe

a=Serial.read();  // read date and store in a

Serial.println(a); // print in serial monitor


//Living Room
if(a=="49")  // when on button was pressed for living room it showed 49 in serial monitor

{

digitalWrite(livingRoom,HIGH);  // turn on the light

}

if(a=="48")  // when pressing off button

{

digitalWrite(livingRoom,LOW); // turn off the light

}

// Basement
if(a=="50") // when pressing on for basement

{

digitalWrite(basement,HIGH); // turn on

}

if(a=="51") // when pressing off for basement

{

digitalWrite(basement,LOW); // turn off

}


// bed room
if(a=="52")  // when pressing on button for bedroom on app

{

digitalWrite(bedRoom,HIGH); // turn on

}

if(a=="53")   // when pressing off

{

digitalWrite(bedRoom,LOW); // turn off

}

}

}
