# Day 2: Explored about Embedded Programming

## 📚 Today's Learning Goal
Learn about Embedded C Programming
- Know what's Embedded C
- Learn the Differences in syntax of Embedded C and regular C
- Write some code for Arduino or similar MCU to get started

## ✅ What I Learned

### Concept 1: [Embedded C]
- **Definition**: The Programming Language to configure MCUs
- **Why it matters**: Regular C can not be used to write Embedded code Hence Embedded C is used
- **Example**: A basic `Hello World` in Regular C is 
    ```c
    #include<stdio.h>
    void main(void){
        printf("Hello World!");
    }
    ```
    whereas in MCUs, Hello World is often referred to Blinking an LED with the help of a GPIO pin in the MCU. 
    This is a basic code for blinking an LED in Arduino MCU at pin 13
    ```c
    #define LED_PIN 13 

    void setup(){
        pinMode(LED_PIN, OUTPUT);
    }

    void loop(){
        digitalWrite(LED_PIN, HIGH);
        delay(1000);
        digitalWrite(LED_PIN, LOW);
        delay(1000);
    }

    ```



## 🔧 What I Built/Coded


### Project: [Hello World in Embedded World]
- **Objective**: Blinking an LED
- **Hardware Used**:  Arduino UNO MCU
- **Key Code Snippet**:
```c
#define LED_PIN 13 

    void setup(){
        pinMode(LED_PIN, OUTPUT);
    }

    void loop(){
        digitalWrite(LED_PIN, HIGH);
        delay(1000);
        digitalWrite(LED_PIN, LOW);
        delay(1000);
    }

```
- **Result**: Blinked the LED connected to PIN 13 of the Arduino Board with a delay of 1 second


## 📖 Resources Used

- [How to Blink an LED with Arduino](https://youtu.be/FKekzzj5844?si=IOAN2d5XmacBWki3) - Beginner-Friendly YouTube Video to Learn how to Blink an LED using Arduino


## ⏭️ Tomorrow's Plan
- To understand what exactly happens when you write `digitalWrite()`
- To understand what exactly happens when you click the upload button


