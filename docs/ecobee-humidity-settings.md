# Ecobee Humidity Configuration for South Florida

Step-by-step guide to configure humidity control on Ecobee Smart Thermostat Premium and Ecobee3 Lite for South Florida's subtropical climate.

## Access Humidity Settings

**On thermostat:**
1. Tap the menu icon (hamburger, top-right)
2. Go to **Settings** → **Thresholds**
3. Find **Humidity** section

**In app:**
1. Open Ecobee app → tap thermostat
2. Settings → Thresholds → Humidity

## Recommended Settings

### AC Overcool Max

This setting allows the AC to cool 1-2°F below your setpoint to extract additional moisture when humidity is high.

- **Setting**: AC Overcool Max = **2°F**
- **Location**: Settings → Thresholds → AC Overcool Max
- **Default**: Off
- **Why**: When indoor humidity exceeds your target, the AC runs slightly longer to condense more moisture onto the evaporator coil. The 2°F limit prevents your home from getting uncomfortably cold.

### Humidity Setpoint

- **Setting**: 45-50%
- **Default**: 55% or Auto
- **Location**: Main screen → tap humidity reading → set target
- **Why**: Factory default of 55-60% is too high for South Florida. Mold grows actively above 55% RH. Setting to 45-50% provides a safety margin.

### Dehumidifier Control (If Equipped)

If you have a whole-home dehumidifier connected to your system:

- **Mode**: On
- **Max runtime**: 60 minutes per cycle
- **Target**: 45% RH
- **Dehumidifier works with AC**: Yes

### Fan Settings

| Setting | Value | Reason |
|---------|-------|--------|
| Fan minimum on time | 0 min/hr | Prevents re-evaporation of moisture |
| Fan dissipation time | 30 seconds | Short post-cooling fan run |
| Fan control during away | Off | Saves energy, prevents humidity cycling |

> **Important**: The "Circulation" feature (Settings → Fan → Minimum Fan Runtime) sounds helpful but is counterproductive in humid climates. Set to 0.

## Remote Sensor Strategy

Place sensors where humidity problems are worst:
- **Master bedroom**: Ensure sleeping comfort (most people are most sensitive at night)
- **Home office**: Where you spend daytime hours
- **Avoid**: Near bathrooms, kitchens, or exterior doors (temporary humidity spikes skew readings)

### Comfort Settings for Sensors

- **Follow Me**: Enable — only considers sensors in occupied rooms
- **Home Comfort**: Use all sensors during scheduled home periods
- **Sleep Comfort**: Use bedroom sensor only during sleep schedule

## Schedule Template

| Time | Setpoint | Comfort Setting |
|------|---------|----------------|
| 6:00 AM - Wake | 75°F | All sensors |
| 8:00 AM - Away | 78°F | All sensors (maintains humidity control) |
| 5:00 PM - Home | 75°F | All sensors |
| 10:00 PM - Sleep | 76°F | Bedroom sensor only |

## Alerts to Enable

- **High humidity alert**: 55% (sends push notification)
- **Low temperature alert**: 65°F (indicates system failure)
- **Filter reminder**: Monthly (South Florida requires monthly changes in summer)

## Common Ecobee Issues in South Florida

### "Calibrating Sensors" Message Persists
- Sensor battery may be low (CR2032, replace annually)
- Sensor too far from thermostat (max 45 feet line-of-sight)
- Wi-Fi interference near sensor location

### Humidity Reads Higher Than Expected
- Ecobee measures humidity at the thermostat location
- Hallways tend to read lower than rooms with exterior walls
- Place a standalone hygrometer in the worst room to compare

### AC Runs Constantly in July/August
- Normal for South Florida when outdoor temp exceeds 93-95°F
- Verify overcool max is not set above 2°F
- If humidity still high, system may be undersized for the heat load
