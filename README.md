# Wireless Communications: Simplified Path Loss & Doppler Simulation (Lab 3)

This project explores wireless communication principles, focusing on simplified path loss models and Doppler effect simulations. Implemented using GNU Radio Companion (GRC), the simulations include both theoretical and practical experiments.

## Contents

### 1. Simplified Path Loss Model
- **Files**:
  - `lab3.grc`
  - `Lab3Receiver.grc`
  - `Lab3Transmitter.grc`
- **Description**:
  Simulates the simplified path loss model to study signal propagation in different environments.
- **Features**:
  - Adjustable parameters for path loss exponent (𝛾), reference distance (𝑑₀), and frequency.
  - Real-time visualization of received signal power as a function of distance.
- **Key Formula**:
  \[
  \frac{P_r}{P_t} = K \left[\frac{d_0}{d}\right]^\gamma
  \]
  where \( K \) is derived from the Friis transmission equation.

### 2. Doppler Effect Simulation
- **Files**:
  - `Lab 3 Bonus - Receiver.grc`
  - `Lab 3 Bonus - Transmitter.grc`
- **Description**:
  Simulates the Doppler effect to study frequency shifts caused by relative motion between a transmitter and receiver.
- **Features**:
  - Continuous wave radar implementation.
  - Visualization of frequency shifts indicating object movement.
- **Key Formula**:
  \[
  f_D = \frac{\nu \cos\theta}{\lambda}
  \]
  where \( \nu \) is the relative velocity, \( \theta \) is the angle, and \( \lambda \) is the wavelength.

## Practical Experiments

### Path Loss
1. **Objective**:
   - Measure signal power at various distances.
   - Analyze the impact of \( d_0 \) and \( \gamma \) on signal attenuation.
2. **Steps**:
   - Run `Lab3Transmitter.grc` and `Lab3Receiver.grc`.
   - Adjust \( d_0 \), \( \gamma \), and distance using GUI sliders.
   - Observe the effect on signal power.

### Doppler Effect
1. **Objective**:
   - Detect object movement using Doppler shifts.
   - Estimate object speed and range.
2. **Steps**:
   - Use `Lab 3 Bonus - Transmitter.grc` and `Lab 3 Bonus - Receiver.grc`.
   - Implement continuous wave radar using the Osmocom block.
   - Observe frequency shifts and detect motion in the environment.

## Theoretical Questions
1. Derive the path loss exponent \( \gamma \) for a given set of signal measurements.
2. Determine conditions where the simplified path loss model matches the free-space model.
3. Calculate the Doppler frequency shift for various scenarios.

## Bonus (20%)
1. Conduct real-world experiments to measure path loss.
2. Implement a system to detect and visualize object movement using Doppler shifts.

## Dependencies
- **Software**: GNU Radio 3.7 or later.
- **Hardware**:
  - SDR devices (e.g., LimeSDR, USRP).
  - Laptops with sufficient processing power.

## How to Run
1. Open the `.grc` files in GNU Radio Companion.
2. Adjust parameters (e.g., frequency, distance) using the GUI.
3. Observe results in QT GUI sinks or Number sinks.

## References
- Wireless Communications, Andrea Goldsmith, Stanford University, 2005.
- Rappaport Wireless Communications Principles And Practice, Prentice Hall, 2002.
- [Wikipedia: Doppler Effect](https://en.wikipedia.org/wiki/Doppler_effect)
