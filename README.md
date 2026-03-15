This project consists of the design and simulation of an analog electronic circuit for temperature measurement, developed as part of a CAD electronics project. The circuit measures temperature in the range −10 °C to 20 °C using a thermistor-based sensor and visually indicates the temperature interval using LED indicators.

The sensor resistance varies with temperature (11 kΩ–22 kΩ), forming a voltage divider that converts resistance changes into a voltage signal. This signal is then processed through several analog stages built with operational amplifiers (TL082), including a voltage follower, differential amplifier, summing amplifier, and inverting amplifier, in order to scale and adjust the signal to a suitable voltage range.

To detect specific temperature intervals, the processed signal is fed into threshold comparators (LM339). Each comparator corresponds to a temperature range and activates an LED indicator when its threshold is reached. This allows the circuit to visually represent temperature intervals:

below 0 °C

0–10 °C

10–15 °C

above 15 °C

The circuit was designed and validated using OrCAD/PSpice, where several simulation analyses were performed to evaluate its behavior and robustness:

Transient (Time Domain) Analysis

Parametric Sweep

Performance Analysis

Monte Carlo Analysis

Worst-Case Analysis

Additionally, a custom LED model was created in the PSpice Model Editor to accurately simulate the LED behavior in the circuit.

This project demonstrates the use of analog signal conditioning, operational amplifiers, comparator circuits, and electronic simulation techniques for implementing a practical temperature monitoring system.
