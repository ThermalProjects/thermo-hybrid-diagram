flowchart LR

PWM[PWM] --> SYS[Thermal System]
Tamb[T_amb] --> SYS

SYS --> PHYS[Physics Model]
PHYS --> TPHYS[T_phys]

SYS --> NN[NN Residual]

TPHYS --> NN
NN --> DELTA[ΔT]

TPHYS --> SUM[+]
DELTA --> SUM

SUM --> Y[T_hat]
