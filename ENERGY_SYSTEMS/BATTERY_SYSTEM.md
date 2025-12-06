LDM Battery System Overview

The Lunar Dust Mitigator (LDM) uses an ultra-simple, ultra-stable battery subsystem designed only for one purpose:

→ Store excess solar power during the lunar day and release limited backup power during the lunar night.

The system is deliberately minimal.
The LDM is not a rover, a drone, or an active engine — it is a static, decade-scale dust-rounding station, so the battery requirements stay extremely small.

1. System Goals

The battery subsystem is required to:

Provide short-duration power bursts to the O-Machine electrostatic chamber when solar intake is low (dust events, micro-shading, dawn/dusk shadows).

Enable “Night Mode,” if enabled by mission parameters, at very low duty cycle (user-configurable, default OFF).

Avoid deep-cycle degradation over multi-year deployments.

Act as an emergency stabilizer during transient solar fluctuations.

No other functionality is required.

2. Battery Type Selection
Lithium Iron Phosphate (LiFePO₄)

Chosen because:

Extremely long cycle life

Thermal stability in vacuum

No thermal runaway behavior

Tolerates irregular charge/discharge cycles

Performs well under low-load, long-duration trickle usage

Nominal pack size is intentionally small:

Capacity: 40–80 Wh (mission-configurable)

Nominal Voltage: 12 V or 24 V, depending on solar regulator configuration

Cells: Ruggedized, epoxy-potted, vacuum-rated modules

The LDM does not need large-scale energy buffering.

3. Charge Management
MPPT Solar Regulator

A micro-MPPT controller handles:

Main solar input

Over-voltage protection

Under-voltage lockout (UVLO)

Battery thermal derating

Night-mode cutoff logic

Charging Behavior

Aggressive charging during peak lunar daytime (0% → 85%)

Slow topping curve from 85% → 100%

Trickle disabled to extend lifespan

Battery is maintained between 25% and 85% during normal operations
unless night-mode is enabled.

4. Discharge Strategy

Battery power is used for:

Electrostatic Burst Pulsing

Control PCB + Sensor Heartbeat

Night-Mode Minimal Operation

The O-Machine draws rapid micro-bursts of energy, not constant drain.
Total power demand is extremely small.

5. Night-Mode Logic

Night-mode only activates if battery ≥ 75% at sunset.

Night-mode discharge curve:

Battery %	Duty Cycle	Action
100–75%	1% activity	Occasional electrostatic pings
74–50%	0.5%	Minimal operations
< 50%	0%	System sleeps until sunrise

This prevents battery death and guarantees multi-year life.

6. Thermal Management

Because LiFePO₄ cells must remain within safe thermal ranges:

The battery is housed inside the insulated internal chassis, sharing thermal mass with the LDM’s core electronics.

Waste heat from the control board maintains survivable temperatures.

Radiative losses controlled via multi-layer insulation (MLI).

No heaters are needed.

7. Expected Lifespan

With the extremely low cycling load:

➡️ 10–15 years of operational life
even under lunar extremes.

8. Failure Modes & Mitigations
Failure Mode	Mitigation
Battery fails open	Solar direct-pass allows minimal daytime operation
MPPT failure	System defaults to passive mode
Cell imbalance	Internal BMS auto-corrects; duty cycles reduced
Thermal drift	MLI insulation & internal mass buffering

The LDM remains functional at a reduced level even under partial battery failure.

9. Why the Battery Matters for the LDM

The LDM’s performance is cumulative — decades of dust rounding.
Missing a few hours or even days is irrelevant.

The battery ensures:

No dead time during shadows

Smooth operation

Night activity if desired

Long-term stability

The system does not depend on perfect uptime — only longevity.
