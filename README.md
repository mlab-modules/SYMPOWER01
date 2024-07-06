### SYMPOWER01  - symmetric power supply

The SYMPOWER01 module is designed to provide symmetric power supply outputs. This module leverages several key components to ensure efficient and reliable power conversion. This documentation outlines the specifications, usage, and key features of the SYMPOWER01 module.

#### Features
- **Input Voltage Range:** 2.8V to 17.5V
- **Output Voltage Options:** Configurable for various symmetric outputs
- **Low Noise Operation:** Utilizes slew rate control to minimize electromagnetic interference (EMI)
- **Current Limiting and Overtemperature Protection:** Ensures safe operation under various conditions
- **Synchronization Capability:** Can synchronize with an external clock for precise control

#### Key Components
1. **LT3439 - Slew Rate Controlled Ultralow Noise DC/DC Transformer Driver**
   - **Function:** Provides low noise and EMI reduction by controlling the output switch voltage and current slew rates.
   - **Features:**
     - Input Voltage Range: 2.8V to 17.5V
     - Low Shutdown Current: <20µA
     - Overcurrent and Overtemperature Protection
     - Synchronizable to external clock
   - **Applications:**
     - Medical instruments
     - Precision instruments
     - Low noise isolated supplies

2. **LT1761 - Low Noise LDO Regulator**
   - **Function:** Provides a regulated low noise output voltage.
   - **Features:**
     - Input Voltage Range: 1.8V to 20V
     - Output Voltage: 1.22V to 15V
     - Low Dropout Voltage
     - Low Noise: 20µV RMS
     - Low Quiescent Current: 30µA

3. **LT1964 - Low Noise, Negative LDO Regulator**
   - **Function:** Provides a regulated negative voltage output.
   - **Features:**
     - Input Voltage Range: -0.9V to -20V
     - Adjustable Output Voltage
     - Low Dropout Voltage: 340mV
     - Low Noise: 30µV RMS
     - Low Quiescent Current: 30µA

4. **SPW7170 - Power MOSFET**
   - **Function:** High-efficiency power switching component.
   - **Features:**
     - Low on-resistance
     - High current handling capability
     - Fast switching speed

5. **FDD03 - DC-DC Converter**
   - **Function:** Provides isolated DC-DC conversion.
   - **Features:**
     - High efficiency
     - Low noise
     - Isolated outputs for safe and versatile applications

#### Typical Application Circuit
The following is a typical application circuit for the SYMPOWER01 module using the LT3439, LT1761, LT1964, SPW7170, and FDD03 components.

```
VIN (2.8V to 17.5V) -> LT3439 -> Transformer -> LT1761 / LT1964 -> VOUT (+5V / -5V)

Key Connections:
- LT3439 provides initial conversion and noise reduction.
- LT1761 regulates the positive output.
- LT1964 regulates the negative output.
- SPW7170 ensures efficient switching.
- FDD03 provides isolated DC-DC conversion if required.
```

#### Design Files
The design files for the SYMPOWER01 module, including schematics, PCB layouts, and BOM, are available in the repository. Ensure you review these files to understand the detailed design and component placement.

### References
- [LT3439 Datasheet](file-XdwirBq84ZO5KzAidt62BNby)
- [LT1761 Datasheet](file-AJWwrKhR4CriuaZMG4m7q3BJ)
- [LT1964 Datasheet](file-FfS7NBOGRbhTVxLaKd6E5epQ)
- [SPW7170 Datasheet](file-oKOMv09CtUxSAOP2BjKTXFYz)
- [FDD03 Datasheet](file-q2bh9hDbYwFTy7T6PSDSZ23N)

For further details, please refer to the provided datasheets and design files.
