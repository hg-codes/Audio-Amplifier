# Audio Amplifier Project

## Overview

This project is an audio amplifier circuit designed to process and amplify audio signals. The circuit consists of multiple stages, including a pre-amplifier, a common emitter amplifier, an active bandpass filter, and a power amplifier. The main goal is to enhance low-power audio signals and drive a speaker or similar load.

## Circuit Description

### 1. **Pre-Amplifier**

- Uses **BC547B** transistors (Q1, Q2) for initial signal amplification.
- R1 and R2 (14kΩ each) set the biasing.
- C1 (22µF) couples the amplified signal to the next stage.

### 2. **Common Emitter Amplifier**

- **Q3 (BC547B)** acts as the main amplifier.
- R4 (13.3MΩ) and R5 (3.3MΩ) provide biasing and gain control.
- Rc1 (28kΩ) and Re1 (1kΩ) control the gain and stability.
- C2 (1nF) helps with frequency stability.

### 3. **Active Band Pass Filter**

- **U2 (UA741 op-amp)** is used to filter specific frequency components.
- R6 and R7 (1.8MΩ each) define the filter characteristics.
- C4 (4nF) and C5 (4pF) set the cutoff frequencies.
- Operates with a **±12V power supply**.

### 4. **Power Amplifier Class AB**

- **Q4 (TIP31A) and Q5 (TIP32)** form a complementary push-pull amplifier.
- D1 and D2 (**1N4148 diodes**) ensure proper biasing.
- R8 and R9 (1kΩ each) limit current.
- C6 and C7 (100µF each) handle power smoothing.
- The output is connected to **RL (12Ω load)**, typically a speaker.

## Power Supply

- **±12V** for the bandpass filter.
- **+5V and -5V** for the power Amplifier and earlier stages.

## Additional Documentation

A document specifying all requirements for this project has also been uploaded. [Check Here](link.com)

## Simulation and Testing

The circuit was simulated using **LTSPICE** to verify gain, frequency response, and output power. Testing involved:

- Injecting a **1 kHz sine wave** as the input signal.
- Measuring gain at different stages.
- Checking the filtered output.
- Ensuring the final amplifier can drive a speaker effectively.

## Conclusion

This audio amplifier successfully amplifies low-power signals(10mV-20mV) while filtering unwanted frequencies. The design balances gain, stability, and efficiency for real-world applications.

## Future Improvements

- Adding a **tone control circuit** to adjust bass and treble.
- Reducing noise by optimizing component values and PCB layout.

### Authors:

- **[Harshit Goyal](https://github.com/hg-codes)**
- **[Manikya Pant](https://github.com/ManikyaPant)**
