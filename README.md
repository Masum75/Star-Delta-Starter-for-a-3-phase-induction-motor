# Star-Delta-Starter-for-a-3-phase-induction-motor

I have implemented a Star-Delta Starter for a 3-phase induction motor using Siemens S7-1200 PLC in TIA Portal V18 and WinCC RT Advanced.

🔹 How the Project Works:
✅ The system consists of three contactors: Main, Star, and Delta.
✅ When power is ON, Main and Star contactors close, starting the motor in star connection.
✅ After 8 seconds, the Star contactor opens and the Delta contactor closes, switching the motor to delta connection for normal operation.
✅ The process is fully automated using PLC logic, with a SCADA interface for monitoring and control.

🔹 Why Use a Star-Delta Starter for Induction Motors?

⚡ The Problem: High Inrush Current in Direct-On-Line (DOL) Start
When a motor is started with a Direct-On-Line (DOL) starter, it draws a very high starting current (6-8 times the full load current) due to lack of back emf at starting, which can:
🔹 Cause voltage drops in the electrical network.
🔹 Damage motor windings due to excessive heating.
🔹 Affect other equipment connected to the same power system.

✅ The Solution: Star-Delta Starter (Reduced Voltage Start)
A Star-Delta Starter reduces the inrush current by first starting the motor in a star (Y) connection and then switching it to a delta (Δ) connection after a short delay.

🛠️ How Does the Star-Delta Starter Work?
1️⃣ Star Connection (Startup Mode):

The three motor windings are connected in a star (Y) configuration.
This reduces the voltage across each winding to 1/√3 (58%) of the supply voltage.
As a result, the starting current is reduced to 1/3 of what it would be in a direct start.
The motor generates low torque, but starts smoothly with reduced electrical and mechanical stress.
2️⃣ Delta Connection (Running Mode):

After a preset delay (8 seconds in my project), the connection switches from star to delta.
The motor now receives the full line voltage across each winding. This allows the motor to operate at full torque and full speed.

🔍 Looking forward to exploring more real-world PLC & SCADA applications! 🚀
