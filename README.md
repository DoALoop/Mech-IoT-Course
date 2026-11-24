# Mech-IoT-Course
Lab notebook for my Mechatronics / IoT Engineering Course

ORIENTATION
How this course works
Twenty weeks, six phases, one capstone: you go from Ohm's law to a secure, multi
node ESP32 system running in Home Assistant. It follows the order an EE/
mechatronics degree teaches it: circuits, then microcontrollers, then sensors and
control, then embedded systems, then networking, then product engineering. Every
day ends with something you built and measured, not something you watched.
PHASE
WEEKS YOU CAN DO THIS AT THE END
COLLEGE COURSE IT
REPLACES
1. Circuits
1–3
Design, draw and build a transistor circuit and predict its
numbers within 10%
Circuits I, Intro to Electronics
2.
Microcontrollers
4–6
Write non-blocking, state-machine firmware that talks
UART, I2C and SPI
Microprocessors / Embedded
I
3. Mechatronics
7–9
Drive DC, servo and stepper motors safely and close a loop
with PID
Mechatronics, Intro to
Controls
4. ESP32 & RTOS
10–12
Ship modular, tested FreeRTOS firmware that sleeps at
microamps
Embedded II, Real-Time
Systems
5. IoT
13–15
Build secure, OTA-updatable devices on MQTT with
dashboards
Computer Networks, IoT
Systems
6. Home &
product
16–18
Integrate devices into Home Assistant and lay out a PCB
Senior Design prep
Capstone
19–20
Deliver a documented system that runs for 7 days
unattended
Senior Design
The weekly rhythm
• 
• 
• 
Mon–Fri, 60–90 min: one daily lab. 20 minutes of theory, 45 minutes of building, 10 minutes writing it up.
Saturday, 3–4 hours: the weekend build. It combines that week's five labs into one working device.
Sunday, 30–60 minutes: reading, review and the exit checks you failed during the week.
Behind schedule? Slip the calendar, never the order. Each week assumes the ones before it.
3
HOW THIS COURSE WORKS
MECHATRONICS & IOT ENGINEERING
How each daily lab is laid out
Every day in the phase tables has three parts:
1. 
2. 
3. 
Concept: what to learn first. Look it up in the reference books or channels listed at the end.
Challenge: what to build. Write your prediction (a number, a waveform, a behaviour) before you power it on.
Exit check: a question or test you must pass without notes. Can't pass it? Redo the lab on Sunday.
Your lab notebook (non-negotiable)
Keep a Git repository with one folder per lab, holding the code, a photo of the build and a 
headings:
• 
• 
• 
• 
• 
• 
Objective
Prediction (with the math)
Schematic (hand-drawn photo in Phase 1, KiCad from Week 3 on)
Measured data
Prediction vs. result, and why they differ
Bugs hit and how you found them
This repo is your transcript. By Week 20 it doubles as a portfolio.
Grading yourself
Score each weekend build out of 10. Under 7 means you repeat it before moving on.
CRITERION
README.md with these
POINTS
Works as specified, every time
3
Predictions written first, then checked with the meter
2
Clean wiring and a correct schematic
2
Code is non-blocking, commented and committed
2
Write-up explains one thing that went wrong
1
House rules
• 
• 
• 
• 
No 
delay() after Week 4. Use real timing.
No library for a part until you've read its datasheet. From Week 12, you write at least one driver yourself.
Never wire mains (120 V AC). Every relay or "smart plug" lab in this course switches 5–12 V loads only. Mains
stays theory until you are trained and use certified modules.
ESP32 pins are 3.3 V and not 5 V tolerant. Check this every time a 5 V part touches an ESP32.
