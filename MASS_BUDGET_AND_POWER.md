#️⃣ 1. BASELINE ASSUMPTIONS

System is approximately shoebox-sized

Passive-first architecture with minimal moving parts

No motors, wheels, or mechanical actuators

Electrostatic chamber drives dust rounding

Small O₂/H₂/He tanks (low-pressure) for emergency utility only

Single solar panel, battery storage, and microcontroller

Designed for multi-year unattended lunar operation

Target total mass: 2.5–5.0 kg depending on variant.

#️⃣ 2. MASS BUDGET (ESTIMATED)
Subsystem	Component	Mass (g)	Notes
Structure	Outer shell (polymer composite)	450	Dust-shedding geometry
	Internal rib cage	300	Shock absorption from landing
	Crushable landing feet	150	Open-cell polymer or aluminum honeycomb
Electrostatic Chamber	Main chamber body	250	Insulators + abrasion lining
	Electrode array	120	Thin metallic plates or wires
	Power modulation board	80	HV step-up converter
Electronics	MCU + flight board	45	Simple ARM-class controller
	IMU	12	Orientation & boot logic
	Environmental sensors	25	Temp, dust, battery
	Safety discharge circuit	18	Prevents charge buildup
Power System	Solar panel (flex)	180	3–5 W peak range
	Battery (LiFePO4, 20–40 Wh)	300	Cold-tolerant chemistry
	Wiring + shielding	90	EMI protection
Gas & Utility Tanks	Low-pressure O₂ tank	120	Refrigerator-sized in concept, scaled here
	Micro He tank	40	Tiny contingency reserve
	Micro H₂ tank	40	Same as above
Thermal System	Radiator coating + insulation	150	Regulates chamber & board temp
Misc	Sealants, fasteners, gaskets	80	Typical allowance
	Margin (10–15%)	300–500	Standard aerospace practice
Total Estimated Mass:

≈ 3.0–4.0 kg depending on configuration

This is well within small-instrument payload envelopes.

#️⃣ 3. POWER GENERATION CAPABILITY
Solar Panel

Area: ~200–250 cm² (flex panel)

Efficiency: 18–22%

Lunar solar constant: ~1360 W/m²

Peak expected output:
3–5 W (depending on angle)

Battery

Capacity: 20–40 Wh

LiFePO4 chosen for:

High cycle life

Superior cold-temperature stability

Lower fire risk vs Li-ion

Night survival requires extreme power discipline.

#️⃣ 4. POWER CONSUMPTION BY SUBSYSTEM
Subsystem	Mode	Power Draw
MCU	Active	50–120 mW
	Sleep	5–10 mW
Environmental sensors	Active	10–30 mW
	Sleep	<1 mW
Electrode Chamber	High frequency	1.5–2.5 W
	Medium	0.8–1.5 W
	Low	0.4–0.8 W
	Idle	<50 mW
Safety discharge	When triggered	100–300 mW
Front dust-repulsor	Pulse	0.5–1.0 W (short-duration)
Thermal pads (rare)	Emergency only	1–2 W

The electrostatic chamber is the dominant load, which is intentional and acceptable.

#️⃣ 5. OPERATING MODES SUMMARY
Day Mode (normal)

Solar provides 3–5 W

Battery tops off

Chamber runs medium–high bursts

Idle periods interleaved for heat control

Energy-positive state.

Night Mode (survival)

Night = 14 Earth days

Rules:

No chamber unless energy surplus

MCU in deep sleep

Wake checks every 4 hrs

90–95% reduction in consumption vs day mode

Heaters forbidden unless below critical threshold

Night is energy-negative but survivable with good daytime charging.

#️⃣ 6. EXPECTED DUTY CYCLES
Under high dust conditions:

60–80% active runtime during the day

High-value burst periods

Moderate battery drain at night

Under low dust conditions:

20–40% active runtime during the day

Extended idle cycles

Night survival easier

Overall system lifespan increases significantly

#️⃣ 7. LIFETIME ENERGY MODEL

Assuming:

~20 Wh battery

~3.5 W sunlight average

Active chamber bursts at ~1.5 W duty

Estimate:

Operational lifetime: 5–20 years
(Depends on dust density, sunlight, electrode wear)

The system is intentionally simple, with no motors, wheels, or complex mechanisms to fail.
