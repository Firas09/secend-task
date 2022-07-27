# secend-task
ok we are going to make a latching system with arduino to automate switshing on and off

1ST what we need to make the circut

Microcontroller or Development Board, for example: ESP32 Dev Board (read ESP32 boards review) ESP8266 NodeMCU (read ESP8266 boards review) Arduino UNO (read best Arduino Starter Kits) NDP6020P Transistor P-Channel MOSFET 2N3904 Transistor BJT NPN Resistors: 220K Ohm, 2x 100K Ohm, 10K Ohm, and 220 Ohm 2x Diodes (for example: 1N5819) Switch/Pushbutton 5V Power Supply

2ND here is the code for the arduino
// Define power latch pin for ESP32 (GPIO 5) / ESP8266 (GPIO 5) / Arduino (Digital 5) const int powerLatch = 5;

void setup() { // Define pin as an OUTPUT pinMode(powerLatch, OUTPUT);

// Keeps the circuit on digitalWrite(powerLatch, HIGH); // Waits for 10 seconds delay(10000); // Turns the power latch circuit off digitalWrite(powerLatch, LOW); }

void loop() {

}
