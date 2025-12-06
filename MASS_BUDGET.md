Lunar Dust Mitigator (LDM) — Preliminary Mass Budget

This document outlines a conservative first-pass mass budget for the autonomous Lunar Dust Mitigator (LDM). The purpose is not to finalize engineering, but to provide a clear, modular estimate that mission designers can refine or scale based on their hardware choices.

All values are intentionally realistic but flexible.

1. TOTAL MASS TARGET

Estimated system mass: 8–14 kg

This range is chosen to keep the system:

Robust enough to survive impact

Light enough for cheap deployment

Compatible with “jettison-from-lander” releases

Scalable for multi-unit habitat arrays

2. MASS BREAKDOWN BY SUBSYSTEM
2.1 Structural Chassis

Materials: Aluminum alloy + dust-resistant coatings

Mass: 2.0–3.0 kg

2.2 Electrostatic Chamber (“O-Machine”)

Randomized-burst electrode matrix

Internal conductor rods

Insulating walls

Mass: 1.0–1.5 kg

2.3 Solar Panel Assembly

Upper chassis panel(s)

Folded or rigid

Mass: 0.8–1.5 kg

2.4 Battery Pack

150–250 Wh LiFePO₄ or similar

Mass: 0.7–1.2 kg

2.5 Microcontroller + Sensor Suite

Includes:

MCU

IMU

Dust ingress sensors

Temperature/health monitors

Mass: 0.2–0.5 kg

2.6 Electrostatic Repulsor Front Plate

Conductive shield plate

Self-cleaning electrode traces

Mass: 0.3–0.6 kg

2.7 Deployment & Landing Hardware

Includes:

Crushable energy-absorbing feet or sled

Lightweight impact cage

Burst-suppression foam interior

Mass: 1.5–3.0 kg

2.8 Cables, Connectors, Fasteners

Mass: 0.2–0.4 kg

3. MASS SUMMARY TABLE
Subsystem	Estimated Mass
Structural Chassis	2.0–3.0 kg
Electrostatic Chamber	1.0–1.5 kg
Solar Panels	0.8–1.5 kg
Battery Pack	0.7–1.2 kg
MCU + Sensors	0.2–0.5 kg
Repulsor Front Plate	0.3–0.6 kg
Landing Hardware	1.5–3.0 kg
Cables/Fasteners	0.2–0.4 kg
TOTAL	7.7–12.7 kg

Round to 8–14 kg to allow scope for future revisions.

4. PRINCIPLES BEHIND MASS DISTRIBUTION

Impact Survivability Comes First
The LDM must survive a ~3–6 m/s terminal impact from low-altitude autonomous deployment.

Center of Mass Must Favor Stability
The O-Machine and battery are intentionally low-mounted.

Minimize “fluffy” components
No hinges, no robotic arms, no motors.
Less mass = fewer failure modes.

Scalable Architecture
Mass distribution remains stable whether the unit is:

5 kg (micro-version)

20+ kg (high-output variant)

5. WHAT THIS FILE ENABLES

With this mass budget in place, engineers can now:

Calculate drop dynamics

Design brackets for rover/lander deployment

Estimate shipping and launch costs

Infer structural load paths

Begin CFD/dust simulations with realistic geometry

Evaluate alternative materials or protective shells
