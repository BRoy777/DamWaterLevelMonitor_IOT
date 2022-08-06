IOT

This is the code for a Dam Water Level Monitoring System which works with NodeMCU 1.0 and ThingSpeak
This code needs to be uploaded in NodeMcu and ThingSpeak data and wifi details in code needs to be changed 
for successful operation.

CODE DESCRIPTION

• ESP8266WIFI library provides ESP8266 specific WiFi routines that we are calling to
connect to the network.
• Const char* ssid means the SSID (name) of the WiFi network you want to connect to
const char*
• Const char* password- the password() function verifies or changes the username
password or the password phrase. The oldpass is the current password or password
phrase for user username ,and is a NULL-terminated character string of a password or
a password phrase.
• Different digital pin numbers are used according to the LEDs, the buzzer and the
ultrasonic sensors trigger and echo pins.
• Serial.begin(115200); passes the value 115200 to the speed parameter. This tells the
Arduino to get ready to exchange messages with the serial monitor at a data rate of
115200 bits per second. That’s 115200 binary ones or zeros per second, and is
commonly called baud rate.
• WiFi.begin-initializes the WiFi library’s network settings and provides the current
status.

• WiFi.status()!=WL_CONNECTED-assigned when connected to WiFi network.
• Server.begin tells the server to begin listening for incoming connections.
• After this the void loop starts and the required functions are defined like
measure() where the measurement details are coded and internet() function is
also is defined where the details of depth of water is updated to the thingspeak.
• digitalWrite() function is used to write a HIGH or LOW value to a digital pin. If a pin
has been configured as output with pinMode(),its voltage will be set to the
corresponding value 3.3 V for HIGH ,0V (ground) for LOW.

• Client disconnected means that the client initiated a request but then disconnected
before it bothered to read all the response.