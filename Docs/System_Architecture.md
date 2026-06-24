# System Architecture

```text
MPU6050 Sensor
      │
      ▼
ESP32 Microcontroller
      │
      ▼
MQTT Broker
      │
      ▼
Python Server
      │
      ▼
TinyML Model
      │
      ▼
Maintenance Recommendation Engine
```

## Data Flow

1. MPU6050 collects vibration data.
2. ESP32 reads sensor values.
3. Data is transmitted via MQTT.
4. Python server receives data.
5. TinyML model detects anomalies.
6. AI generates maintenance recommendations.
