# Arduino MPU6500 Register-Level IMU Driver

This repository contains a **register-level C++ driver implementation for the MPU-6500 IMU on an Arduino platform**, built directly from the official datasheet without relying on high-level libraries.

The project implements **low-level I²C communication**, sequential register reads, and conversion of raw 16-bit accelerometer and gyroscope data into physical units (g and deg/s). Using this data, a **complementary filter is applied to estimate roll and pitch**, blending short-term gyroscope integration with long-term accelerometer stability.

This project serves as a strong foundation for **sensor fusion and state estimation**, enabling future extensions such as Kalman filtering, attitude estimation, and closed-loop control systems.
