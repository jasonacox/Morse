# Morse

Arduino library to send Morse Code dots and dashes on a specified pin.

## Description

This is a simple Arduino library used to demonstrate how you can extend the functionality of Arduino.

This library example is used in the [Writing a Library for Arduino tutorial](https://docs.arduino.cc/learn/contributions/arduino-creating-library-guide).

## Example

Here is an example sketch used to send the SOS distress call.

```cpp
#include "Morse.h"

Morse morse(13);

void setup()
{
  morse.begin(); 
}

void loop()
{
  morse.dot(); morse.dot(); morse.dot();
  morse.dash(); morse.dash(); morse.dash();
  morse.dot(); morse.dot(); morse.dot();
  delay(3000);
}
```
