# Intelligent-Traffic-Management-System-using-ANPR-and-ATCC

# Introduction
This project implements an Intelligent Traffic Management System using ANPR (Automatic Number Plate Recognition) and ATCC (Automatic Traffic Classification and Control). It integrates computer vision, real-time data processing, and automated detection to improve road safety, streamline traffic regulation, and support smart-city infrastructure.

# Problem Statement
Traffic Congestion: Long queues cause fuel wastage and increased pollution.
Inefficient Monitoring: Heavy manual work leads to delays, errors, and inconsistent tracking.
Violation Detection Challenges: Speeding, signal jumping, and other violations often go unnoticed.
Security Risks: Tracking vehicles involved in crime remains difficult in manual processes.

# System Architecture (Dashboard Overview)
1. Login Page
Allows authenticated users to log in with secure credentials.

2. Dashboard (Home Page)
Provides project overview and navigation buttons:
Search
Live Monitoring
Upload Videos
Results
Logout

4. Live Monitoring
Supports ANPR and ATCC with multiple camera inputs.
Users can upload videos or provide IP camera streams.

# ANPR Module
Detects vehicle license plates
Performs OCR using PyTesseract.
Stores extracted plate number, timestamp, and vehicle image in the database.

# ATCC Module
Performs live vehicle counting and classification.
Supports real-time monitoring.
Enables dynamic traffic light switching based on vehicle density.

# Model Uniqueness & Additional Features
Heatmap Visualization – Detects congestion using directional vectors.
Helmet Detection – Identifies riders without helmets.
Accident Detection – Detects collisions or sudden stops.
Triple Riding Detection – Identifies more than two riders on a motorcycle.
Dynamic Traffic Light Switching – Automatically adjusts signal timing.
Signal Jumping Detection – Detects violations and stores plate number, time, and date.
Video Upload Console – User uploads help create training datasets for improved accuracy.

# Technologies Used
Frontend
HTML, CSS, JavaScript
Backend
Flask (Python Web Framework)
Python for CV, ML, and OCR
OpenCV, YOLOv8 – Vehicle detection, classification, and movement tracking
PyTesseract – Number plate recognition
MySQL – Data storage and retrieval
TensorFlow – ML model implementation
Dynamic Graphs & Heatmaps – Visualizing traffic patterns
Threading & OS Modules – System-level operations

# Applications
Traffic Management: Real-time vehicle monitoring and flow optimization.
Toll Collection: Automated payment using ANPR.
Law Enforcement: Detects stolen or suspicious vehicles and tracks violations.
Urban Planning: Traffic pattern analysis aids infrastructure design.
Parking Management: Tracks vehicle entry and exit.
Surveillance: Enhances security in restricted zones.

# Future Work
Real-time Alerts: SMS/notifications for violations, accidents, and congestion.
Advanced Dashboard: Heatmaps, simulation, congestion points for planners.
Hardware Integration: IoT-enabled smart signals and sensors.
AI Enhancements: Deep learning for adaptive traffic control.
Advanced Analytics: Predictive analysis for traffic behavior and violations.

# Application Outcome
The system presents a modern, automated solution to urban traffic challenges using advanced computer vision and AI. It significantly enhances traffic efficiency, road safety, and law enforcement through intelligent monitoring and real-time insights.

# Challenges Faced
Integrating multiple functionalities into one system.
Lack of good-quality training/testing data → Solved using PyTesseract for efficient extraction.
Local storage limitations during video processing → Solved by splitting videos into chunks and processing only relevant segments.

# Key Considerations
Speeding Detection: Achieved using Heatmap Visualization to spot rash or zigzag driving.
Vehicle Classes: Custom-defined classes for all vehicle types including trucks, cars, motorcycles, etc.

# Contributions
Contributions, improvements, and suggestions are welcome! Feel free to open issues or submit pull requests.
