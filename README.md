# Air-quality-monitor-
An Air Quality Monitoring System is used to monitor air pollution levels using parameters such as AQI, gas concentration, and temperature. The Python program analyzes the entered sensor values and displays the air quality as Good, Moderate, Poor, or Hazardous.
# Air Quality Monitoring System

print("===== AIR QUALITY MONITORING SYSTEM =====")

aqi = float(input("Enter AQI value: "))
temperature = float(input("Enter temperature (°C): "))

print("\n----- Air Quality Report -----")
print("AQI:", aqi)
print("Temperature:", temperature, "°C")

if aqi <= 50:
    status = "GOOD"
elif aqi <= 100:
    status = "MODERATE"
elif aqi <= 200:
    status = "POOR"
elif aqi <= 300:
    status = "VERY POOR"
else:
    status = "HAZARDOUS"

print("Air Quality:", status)

if status == "GOOD":
    print("Air quality is good.")
elif status == "MODERATE":
    print("Air quality is acceptable.")
elif status == "POOR":
    print("Warning: Air pollution level is high.")
elif status == "VERY POOR":
    print("Alert: Avoid prolonged outdoor exposure.")
else
