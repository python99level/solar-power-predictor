# solar-power-predictor
AI-powered solar energy prediction system developed in Python to estimate electricity generation and optimize renewable energy usage.
import math

# Solar panel specifications
panel_power = 550  # Watts
number_of_panels = 20
sun_hours = 7      # Average sunlight hours per day
efficiency = 0.85  # System efficiency

# Daily production
daily_energy = (
    panel_power *
    number_of_panels *
    sun_hours *
    efficiency
) / 1000  # kWh

# Monthly and yearly production
monthly_energy = daily_energy * 30
yearly_energy = daily_energy * 365

print("Solar Energy Production")
print("----------------------")
print(f"Daily Production: {daily_energy:.2f} kWh")
print(f"Monthly Production: {monthly_energy:.2f} kWh")
print(f"Yearly Production: {yearly_energy:.2f} kWh")
