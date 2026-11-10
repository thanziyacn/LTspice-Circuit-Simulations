# Experiment 01 — Basic DC Resistive Circuit

**Project:** LTspice – Analog Electronics Learning Journey  
**Simulation Tool:** LTspice  
**Circuit Type:** DC resistive circuit  
**Analysis:** Transient analysis (`.tran 1`)

## 1. Why I Started Here

Before exploring semiconductor devices and complex analog circuits, I wanted to understand how a simple DC circuit behaves in a simulation environment.

I started with a basic voltage source and resistor to connect the concept of Ohm’s Law from classroom learning with practical circuit simulation.

## 2. The Question ? 

If a 10 V DC supply is connected across a 1 kΩ resistor:

- What current should flow through the resistor?
- Does the simulated current agree with the theoretical calculation?
- How does a DC current appear in a waveform viewer?

## 3. My Circuit Design

The circuit consists of:

| Component | Value |
|---|---:|
| DC voltage source (V1) | 10 V |
| Resistor (R1) | 1 kΩ |
| Ground | 0 V reference |
| Simulation command | `.tran 1` |

**Circuit configuration:** A 10 V DC source connected in series with a 1 kΩ resistor, with the negative terminal connected to ground.

## 4. Understanding the Mathematics

I used Ohm’s Law to calculate the expected current.
Understanding the Mathematics

To predict the circuit behaviour, I applied Ohm's Law.

V = I × R

Rearranging:

I = V / R

Substituting the selected values:

I = 10 / 1000

Expected current = 10 mA

The expected voltage across the resistor is 10 V.

## 5. Simulation and Verification

I constructed the circuit in LTspice and ran transient analysis using:
''transt ''

The simulation waveform shows a constant current over the 1-second time interval.

**What I observed:**

- The current remains approximately constant at 10 mA in magnitude.
- The voltage source current appears around −10 mA because of LTspice's current reference direction.
- The negative sign represents the direction of current relative to the source's reference convention.
- The resistor current magnitude agrees with the theoretical value of 10 mA.

## 6. Theory vs Simulation

| Parameter | Theoretical value | Observed in simulation |
|---|---:|---:|
| Supply voltage | 10 V | 10 V |
| Resistance | 1 kΩ | 1 kΩ |
| Current magnitude | 10 mA | Approximately 10 mA |
| Current behaviour | Constant DC | Constant waveform |

## 7. What I Understood

This experiment helped me understand that:

- Ohm’s Law can be verified using circuit simulation.
- A DC circuit produces a constant current under steady operating conditions.
- The waveform viewer helps analyse circuit behaviour over time.
- Current direction and current magnitude are different concepts when interpreting SPICE results.

## 8. What I Want to Explore Next

After understanding a single-resistor circuit, I want to investigate how voltage and current behave when two resistors are connected in series.

My next experiment will focus on a **voltage divider circuit**, including the relationship between resistance values and output voltage.

## 9. Skills Practised

- LTspice schematic creation
- Component placement and wiring
- DC voltage source configuration
- Resistor value configuration
- Transient simulation
- Waveform interpretation
- Applying Ohm’s Law to verify simulation results

---

**Learning note:** This is my first step in connecting analog electronics theory with circuit simulation. I will continue documenting each experiment with its circuit, calculations, simulation evidence, and engineering observations.
