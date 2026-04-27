# BuildCored-Orcas-Day20
I2CPlayground — BUILDCORED ORCAS Day 20

What it does. This script turns your laptop into a real-time data monitor that tracks sound levels, camera movement, and system performance. It displays this data in a live dashboard and automatically flags anomalies whenever one of those sensors detects a sudden, unusual spike.

Hardware concept. The project mimics a Data Acquisition (DAQ) system, which is a professional tool used by engineers to collect physical signals from the real world and convert them into digital data for analysis. Like an industrial DAQ, your script uses a shared clock to ensure every sensor reading is perfectly synced to the exact same timestamp.

What I would do differently. I'd move the sensor-reading logic into multiprocessing instead of threading to prevent the heavy Optical Flow camera math from slowing down the other sensors. 

Run it. python day20_starter.py
