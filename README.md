# 🌿 SmartAir_TX – Real-Time Temperature & Humidity Monitoring (STM32 + FreeRTOS)
# 📌 Overview

SmartAir_TX is a real-time embedded system developed using C (Embedded C) on an STM32 microcontroller with FreeRTOS.
The system reads temperature and humidity data from a DHT11 sensor and displays the output via UART at fixed intervals.

This project demonstrates practical implementation of RTOS concepts and low-level programming using the C language in embedded systems.

# 🎯 Features

🌡️ Real-time Temperature Monitoring

💧 Real-time Humidity Monitoring

⏱️ Periodic execution (every 3 seconds) using FreeRTOS software timer

🔄 Multi-tasking with FreeRTOS

📦 Queue-based inter-task communication

🔐 Semaphore for synchronization

🛡️ Mutex for safe UART access

📡 UART output

# 🛠️ Tech Stack

Programming Language: C (Embedded C)

Microcontroller: STM32

RTOS: FreeRTOS

Sensor: DHT11

Communication: UART

# 🧠 System Architecture

# 🔹 Tasks

# SensorTask

Reads temperature & humidity using DHT11

Waits for semaphore signal

Sends data to queue

# PrintTask

Receives data from queue

Prints via UART using mutex

🔹 RTOS Components

Queue → Data transfer between tasks

Semaphore → Synchronization

Mutex → UART protection

Timer → 3-second periodic trigger

# 📤 Output

Temperature -> 28

Humidity -> 65

# 🔌 Hardware Requirements

STM32 Board

DHT11 Sensor

UART 

# 📈 Learning Outcomes

Strong understanding of C in embedded systems

Hands-on experience with FreeRTOS

Real-time task scheduling and synchronization

Sensor interfacing and UART communication
