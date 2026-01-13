# PNC – Parametric Nozzle Cleaning for Klipper

PNC (Parametric Nozzle Cleaning) is a **universal nozzle cleaning system for Klipper-based 3D printers**.  
It provides multiple parametric cleaning patterns with clear separation between configuration and execution.

PNC is designed to be:
- machine-agnostic
- safe by design
- easy to calibrate
- easy to extend

No slicer tricks.  
No hardcoded values.  
Just predictable, parametric motion.

## ✨ Features

- Multiple cleaning patterns:
  - **SAW** – directional, aggressive
  - **W** – general-purpose
  - **BOX** – contact-heavy, pressure-based
- Fully parametric configuration
- Independent speed and geometry per pattern
- One global travel system (no contact)
- Safe Z handling for all moves
- Clean and documented configuration
- Compatible with all Klipper machines

## 🧠 Design Philosophy

PNC follows a few simple rules:

- Travel speed does not clean anything
- Cleaning efficiency comes from contact time and pressure
- Each pattern has a specific mechanical purpose
- Configuration should explain *what to change* and *why*

The goal is not to be the fastest, but the most **predictable and tunable**.

## 📦 Installation

1. Copy `PNC.cfg` into your Klipper configuration directory  
2. Include it in `printer.cfg`:
