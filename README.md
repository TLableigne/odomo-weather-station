# Odomo

Odomo is a Java-based home automation and weather monitoring terminal application. It displays real-time weather data (indoor/outdoor temperature, humidity, atmospheric pressure, sunshine, wind speed and direction) and heating status in a text-based ASCII interface.

## Requirements

- Java JDK (Java 17 or higher recommended)
- Apache Ant

## How to Compile & Run

### Using Apache Ant

1. **Compile the project:**
   ```bash
   ant compile
   ```

2. **Run the application:**
   ```bash
   ant run
   ```

### Manual Compilation & Execution

1. Compile source files:
   ```bash
   javac -d build/classes src/odomo/*.java
   ```

2. Run the application:
   ```bash
   java -cp build/classes odomo.Odomo
   ```

## How to Use

When you launch Odomo, an interactive terminal interface displays the status screen with current sensor metrics and a text-based graph/histogram. 

At the `Action : ` prompt, enter one of the following single-character commands:

- **A** : Show help instructions.
- **M** or **P** : Switch to Weather mode (displays 24-hour precipitation/pluviometry histogram).
- **T** : Switch to Weather mode displaying the temperature histogram for the last 60 minutes.
- **C** : Switch to Heating mode.
- **N** : Modify heating time slots (Normal mode heating schedule entry).
- **Q** : Quit the application.
