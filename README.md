# 💧 AquaGuardian: Smart Water Drinking Reminder System

### An Embedded Systems Mini Project Using LPC2148

AquaGuardian is an embedded-based smart water drinking reminder system designed to encourage regular water consumption and help users maintain their daily hydration goals.

The system uses an LPC2148 microcontroller, a Real-Time Clock (RTC), an LCD display, and input devices to track water intake and remind users to drink water at regular intervals.

## 📌 Project Overview

Many people forget to drink water regularly because of busy schedules and work routines. AquaGuardian addresses this problem by providing periodic reminders and tracking daily water consumption.

The user can configure a daily drinking target, record water intake, and monitor the remaining target through an LCD interface.

## 🎯 Objectives

* Encourage regular water consumption.
* Allow users to set a daily water intake target.
* Track the number of recorded drinking events.
* Display the remaining target on an LCD.
* Provide reminders using a buzzer.
* Use an RTC to manage time-based reminders and daily tracking.
* Reset daily consumption when a new day begins.

## ✨ Features

* **Daily Target Configuration:** Set a daily water intake target using a keypad.
* **Water Intake Tracking:** Record water consumption using a push button.
* **Real-Time Clock:** Maintain time and date for reminder scheduling.
* **Periodic Reminders:** Generate reminders at configured intervals.
* **LCD Display:** Show the current time, daily target, consumption, and remaining target.
* **LED Indication:**

  * 🟢 Green LED — Daily target achieved.
  * 🟡 Yellow LED — Progress has reached the configured intermediate level.
  * 🔴 Red LED — Target not achieved, according to the programmed status logic.
* **Buzzer Alert:** Provide an audible reminder.
* **Daily Reset:** Start a new daily tracking cycle when the date changes.
* **Keypad Interface:** Configure settings through a 4×4 matrix keypad.

## 🛠️ Hardware Components

| Component               | Purpose                                 |
| ----------------------- | --------------------------------------- |
| LPC2148 Microcontroller | Main controller                         |
| 16×2 LCD                | Display system information              |
| 4×4 Matrix Keypad       | User input and configuration            |
| Real-Time Clock (RTC)   | Time and date management                |
| Push Buttons            | Record water intake and access settings |
| Buzzer                  | Audible reminders                       |
| LEDs                    | Indicate progress and target status     |
| Connecting Wires        | Hardware interconnections               |
| Power Supply            | Supply power to the circuit             |

## 💻 Software Requirements

* Embedded C
* Keil µVision IDE
* Proteus Design Suite
* LPC2148 microcontroller support
* Suitable startup files and device header files

## ⚙️ Working Principle

1. **System Initialization:** The LPC2148 initializes the GPIO pins, LCD, keypad, RTC, LEDs, and buzzer.
2. **Target Configuration:** The user configures the daily water intake target through the keypad.
3. **Water Intake Recording:** When the user drinks water, they press the designated push button to record the event.
4. **Consumption Calculation:** The controller updates the recorded consumption and calculates the remaining target.
5. **Display Update:** The LCD displays the latest tracking information.
6. **Periodic Reminder:** The system checks the configured reminder interval and activates the buzzer when a reminder is due.
7. **Progress Indication:** LEDs indicate the user's progress according to the programmed conditions.
8. **Daily Reset:** When a new day is detected, the system resets the daily consumption count.

## 🔄 System Flow

       START
         |
         v
 Initialize LPC2148
         |
         v
 Initialize LCD, RTC,
 Keypad, GPIO and Buzzer
         |
         v
 Set Daily Water Target
         |
         v
 Read RTC Time and Date
         |
         v
 Check User Input
         |
         v
 Record Water Intake
         |
         v
 Update Consumption
 and Remaining Target
         |
         v
 Update LCD and LEDs
         |
         v
 Check Reminder Interval
         |
         v
 Activate Buzzer if Required
         |
         v
 Check for New Day
         |
         v
 Reset Daily Count if Required
         |
         v
 Repeat Main Loop
```

## 🔌 Main Hardware Interfaces

| Interface             | Function                                 |
| --------------------- | ---------------------------------------- |
| GPIO                  | Read buttons and control LEDs and buzzer |
| LCD Interface         | Display tracking information             |
| Matrix Keypad         | Accept user settings                     |
| RTC                   | Provide time and date                    |
| Timer/Delay Functions | Support timing and display operations    |

## 🧪 Testing and Simulation

The project can be developed and tested using Keil µVision and Proteus.

Testing can include:

* Initializing the LCD and displaying system information.
* Setting and updating the daily target.
* Recording water intake.
* Verifying the remaining-target calculation.
* Checking reminder timing.
* Testing buzzer and LED indications.
* Verifying daily reset functionality.

## 🚀 Future Enhancements

* Add a real-time water-volume measurement sensor.
* Store daily consumption records in external EEPROM.
* Add GSM notifications for remote reminders.
* Develop a mobile application for tracking hydration.
* Add historical consumption statistics.

## 📚 Learning Outcomes

This project provides practical experience with:

* Embedded C programming.
* LPC2148 microcontroller programming.
* GPIO configuration.
* LCD interfacing.
* Matrix keypad interfacing.
* RTC programming.
* Interrupts and time-based operations.
* Hardware simulation using Proteus.
* Embedded software development using Keil µVision.

## 👨‍💻 Project Information

**Project Name:** AquaGuardian – Smart Water Drinking Reminder System

**Platform:** LPC2148 ARM7 Microcontroller

**Programming Language:** Embedded C

**Development Tools:** Keil µVision and Proteus

**Project Type:** Embedded Systems Mini Project
