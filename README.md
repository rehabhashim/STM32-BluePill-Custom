# STM32-BluePill-Custom
KiCad project for a custom STM32F103C8T6 (Blue Pill) development board. The PCB layout focuses on practical hardware design principles, including power integrity, ground planes, and DFM rules.


Key technical details:

The design centers on the STM32F103C8T6 (ARM Cortex-M3) microcontroller driven by a 16MHz external crystal. For robust power distribution, I implemented solid copper pours for the VBUS and +3.3V nets to improve thermal and current handling, backed by a continuous GND pour across the board to ensure a solid return path and minimize EMI. Signal integrity was prioritized by placing individual 100nF decoupling capacitors directly at the MCU's VDD pins to reduce loop inductance, alongside a dedicated VDDA filter network utilizing a 120Ω ferrite bead and capacitors for clean ADC performance. Mechanically, the board's outline and edge cuts were explicitly engineered to properly overhang the USB-B Mini connector, preventing any physical clearance issues post-fabrication.


<img width="1605" height="835" alt="1" src="https://github.com/user-attachments/assets/97ee374e-2d1e-4e10-a8f6-dc127bf2fb0e" />
<img width="1605" height="835" alt="STM32" src="https://github.com/user-attachments/assets/d1021c3d-4d53-46b1-bb3d-06c9722061c0" />
<img width="427" height="329" alt="Screenshot 2026-09-01 005449" src="https://github.com/user-attachments/assets/b9681ec3-29b2-4f59-9d57-89d1b490afe1" />
