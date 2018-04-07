# maglev-hardware
KiCad schematic and PCB for maglev projects. See preview in `*.pdf` files.

## Theory
In terms of control systems' general theory there're 4 main components: object under control; actuators and drivers; controller itself; feedback loop. Applied to this magnetic levitation system, these components are:
  - Object: permanent magnet
  - Driver: almost this schematic plus PWM
  - Controller: PID algorithm executed by the MCU (see [maglev-ti-rtos](https://github.com/ussserrr/maglev-ti-rtos))
  - Feedback: Hall sensor
We specify setpoint (desired voltage depended on mutual arrangement of permanent and electro magnets) and get status of the process variable by Hall sensor (feedback value).
