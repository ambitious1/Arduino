//Travis D.
//Arduino
//TouchPad Timer
//Fig


// Pin for the LED
//int LEDPin = 13;
// Pin to connect to your drawing
int touchedCutoff = 60;
int firsttime1,firsttime2,firsttime3,firsttime4,firsttime5,firsttime6=1;
unsigned long startTime1,startTime2,startTime3,startTime4,startTime5,startTime6=0;
volatile unsigned long pressTime1,pressTime2,pressTime3,pressTime4,pressTime5,pressTime6=0;
int capSensePin1 = 2;
int capSensePin2 = 3;
int capSensePin3 = 4;
int capSensePin4 = 5;
int capSensePin5 = 6;
int capSensePin6 = 7;
int ledPin = 13;
float h, m, s, ms;
unsigned long over;


void setup()
{
  Serial.begin(9600);
  pinMode(ledPin, OUTPUT);
  pinMode(capSensePin1, INPUT);
  digitalWrite(capSensePin1, HIGH);
  Serial.println("Press 1 for Start/reset, 2 for elapsed time");
  //attachInterrupt(0, displayResult(a,b), RISING);
}

void displayResult(unsigned long a, unsigned long b)
{     
  h = int(a / 3600000);
  over = a % 3600000;
  m = int(over / 60000);
  over = over % 60000;
  s = int(over / 1000);
  ms = over % 1000;

  Serial.print("Formatted Press time: ");
  Serial.print(h, 0);
  Serial.print("h ");
  Serial.print(m, 0);
  Serial.print("m ");
  Serial.print(s, 0);
  Serial.print("s ");
  Serial.print(ms, 0);
  Serial.println("ms");
  Serial.println(); 
}

void loop(){
  // If the capacitive sensor reads above a certain threshold,
  //  turn on the LED
  if (readCapacitivePin(capSensePin1) > touchedCutoff) {
    // digitalWrite(LEDPin, HIGH);
   
    if(digitalRead(capSensePin1) == LOW){
      if(firsttime1 == true){
        startTime1 = millis();

        firsttime1=0;
      }

      pressTime1 = millis() - startTime1;

      if(pressTime1 >= 1){
        Serial.print("Pin2 Runtime: ");
        Serial.print(int(pressTime1/1000));
        Serial.print(" secs ");
        Serial.print(pressTime1);
        Serial.println(" msecs");
        
        Serial.print("<pin2>");
        Serial.print(readCapacitivePin(capSensePin1));
        Serial.println("</pin2>");
        

        displayResult(pressTime1,startTime1); 

      }
      if(pressTime1>3000){
        //digitalWrite(ledPin, HIGH); 
      }
      
    }

    else if(firsttime1 == false){
      firsttime1 = true;
      delay(5);
      Serial.println("Time: 0 milleseconds; 0 seconds");
      // digitalWrite(ledPin, LOW);
    }
  }

  if (readCapacitivePin(capSensePin2) > touchedCutoff) {
    // digitalWrite(LEDPin, HIGH);
    delay(10);
    if(digitalRead(capSensePin2) == LOW){
      if(firsttime2 == true){
        startTime2 = millis();
        firsttime2=0;
      }

      pressTime2 = millis()- startTime2;
      if(pressTime2 >= 1){
        Serial.print("Pin3 Runtime: ");
        Serial.print(int(pressTime2/1000));
        Serial.print(" secs ");
        Serial.print(pressTime2);
        Serial.println(" msecs");

        Serial.print("<pin3>");
        Serial.print(readCapacitivePin(capSensePin2));
        Serial.println("</pin3>");
        
        displayResult(pressTime2,startTime2); 

      }
      if(pressTime2>3000){
        //digitalWrite(ledPin, HIGH); 
      }
    }

    else if(firsttime2 == false){
      firsttime2 = true;

      Serial.println("Time: 0 milleseconds; 0 seconds");
      // digitalWrite(ledPin, LOW);
    }
  }  

  if (readCapacitivePin(capSensePin3) > touchedCutoff) {
    // digitalWrite(LEDPin, HIGH);
    delay(10);
    if(digitalRead(capSensePin3) == LOW){
      if(firsttime3 == true){
        startTime3 = millis();
        firsttime3=0;
      }
      pressTime3 = millis()- startTime3;
      if(pressTime3 >= 1){
        Serial.print("Pin4 Runtime: ");
        Serial.print(int(pressTime3/1000));
        Serial.print(" secs ");
        Serial.print(pressTime3);
        Serial.println(" msecs");

        Serial.print("<pin4>");
        Serial.print(readCapacitivePin(capSensePin3));
        Serial.println("</pin4>");
        
        displayResult(pressTime3,startTime3); 
      }
      if(pressTime3>3000){
        //digitalWrite(ledPin, HIGH); 
      }
    }

    else if(firsttime3 == false){
      firsttime3 = true;

      Serial.println("Time: 0 milleseconds; 0 seconds");
      // digitalWrite(ledPin, LOW);
    }
  }
  if (readCapacitivePin(capSensePin4) > touchedCutoff) {
    // digitalWrite(LEDPin, HIGH);
    delay(10);
    if(digitalRead(capSensePin4) == LOW){
      if(firsttime4 == true){
        startTime4 = millis();
        firsttime4=0;
      }

      pressTime4 = millis()- startTime4;
      if(pressTime4 >= 1){
        Serial.print("Pin5 Runtime: ");
        Serial.print(int(pressTime4/1000));
        Serial.print(" secs ");
        Serial.print(pressTime4);
        Serial.println(" msecs");
        
        Serial.print("<pin5>");
        Serial.print(readCapacitivePin(capSensePin4));
        Serial.println("</pin5>");
        

        displayResult(pressTime4,startTime4); 
      }
      if(pressTime4>3000){
        //digitalWrite(ledPin, HIGH); 
      }
    }

    else if(firsttime4 == false){
      firsttime4 = true;

      Serial.println("Time: 0 milleseconds; 0 seconds");
      // digitalWrite(ledPin, LOW);
    }
  }

  if (readCapacitivePin(capSensePin5) > touchedCutoff) {
    // digitalWrite(LEDPin, HIGH);
    delay(10);
    if(digitalRead(capSensePin5) == LOW){
      if(firsttime5 == true){
        startTime5 = millis();
        firsttime5=0;
      }
      pressTime5 = millis()- startTime5;
      if(pressTime5 >= 1){
        Serial.print("Pin6 Runtime: ");
        Serial.print(int(pressTime5/1000));
        Serial.print(" secs ");
        Serial.print(pressTime5);
        Serial.println(" msecs");
        
        Serial.print("<pin6>");
        Serial.print(readCapacitivePin(capSensePin5));
        Serial.print("</pin6>");
        
        displayResult(pressTime5,startTime5); 
      }
      if(pressTime5>3000){
        //digitalWrite(ledPin, HIGH); 
      }
    }

    else if(firsttime5 == false){
      firsttime5 = true;

      Serial.println("Time: 0 milleseconds; 0 seconds");
      // digitalWrite(ledPin, LOW);
    }
  }
  if (readCapacitivePin(capSensePin6) > touchedCutoff) {
    // digitalWrite(LEDPin, HIGH);
    delay(10);
    if(digitalRead(capSensePin6) == LOW){
      if(firsttime6 == true){
        startTime6 = millis();
        firsttime6=0;
      }
      pressTime6 = millis()- startTime6;
      if(pressTime6 >= 1){
        Serial.print("Pin7 Runtime: ");
        Serial.print(int(pressTime6/1000));
        Serial.print(" secs ");
        Serial.print(pressTime6);
        Serial.println(" msecs");

        Serial.print("<pin7>");
        Serial.print(readCapacitivePin(capSensePin6));
        Serial.print("</pin7>");
        
        displayResult(pressTime6,startTime6); 
      }
      if(pressTime6>3000){
        //digitalWrite(ledPin, HIGH); 
      }
    }

    else if(firsttime6 == false){
      firsttime6 = true;

      Serial.println("Time: 0 milleseconds; 0 seconds");
      // digitalWrite(ledPin, LOW);
    }
  }
}


// readCapacitivePin
//  Input: Arduino pin number
//  Output: A number, from 0 to 17 expressing
//          how much capacitance is on the pin
//  When you touch the pin, or whatever you have
//  attached to it, the number will get higher
//  In order for this to work now,
// The pin should have a 1+Megaohm resistor pulling
//  it up to +5v.
uint8_t readCapacitivePin(int pinToMeasure){
  // This is how you declare a variable which
  //  will hold the PORT, PIN, and DDR registers
  //  on an AVR
  volatile uint8_t* port;
  volatile uint8_t* ddr;
  volatile uint8_t* pin;
  // Here we translate the input pin number from
  //  Arduino pin number to the AVR PORT, PIN, DDR,
  //  and which bit of those registers we care about.
  byte bitmask;
  if ((pinToMeasure >= 0) && (pinToMeasure <= 7)){
    port = &PORTD;
    ddr = &DDRD;
    bitmask = 1 << pinToMeasure;
    pin = &PIND;
  }
  if ((pinToMeasure > 7) && (pinToMeasure <= 13)){
    port = &PORTB;
    ddr = &DDRB;
    bitmask = 1 << (pinToMeasure - 8);
    pin = &PINB;
  }
  if ((pinToMeasure > 13) && (pinToMeasure <= 19)){
    port = &PORTC;
    ddr = &DDRC;
    bitmask = 1 << (pinToMeasure - 13);
    pin = &PINC;
  }
  // Discharge the pin first by setting it low and output
  *port &= ~(bitmask);
  *ddr  |= bitmask;
  delay(1);
  // Make the pin an input WITHOUT the internal pull-up on
  *ddr &= ~(bitmask);
  // Now see how long the pin to get pulled up
  int cycles = 16000;
  for(int i = 0; i < cycles; i++){
    if (*pin & bitmask){
      cycles = i;
      break;
    }
  }
  // Discharge the pin again by setting it low and output
  //  It's important to leave the pins low if you want to 
  //  be able to touch more than 1 sensor at a time - if
  //  the sensor is left pulled high, when you touch
  //  two sensors, your body will transfer the charge between
  //  sensors.
  *port &= ~(bitmask);
  *ddr  |= bitmask;

  return cycles;
}

