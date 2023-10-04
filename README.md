
#include <Ultrasonic.h>

Ultrasonic sensor1(GPIO_TRIGGER1, GPIO_ECHO1);

Ultrasonic sensor2(GPIO_TRIGGER2, GPIO_ECHO2);

// Add more sensors if needed

void setup() {

Serial.begin(115200);

}

void loop() {

long distance1 = sensor1.read();

long distance2 = sensor2.read();

// Read distances from more sensors if needed

// Process distance data and manage parking spaces here

delay(1000); // Delay for better readability

}
