# Google Nest Learning Thermostat — South Florida Schedule Optimization

The Nest Learning Thermostat excels at adapting to your patterns, but its learning algorithm is trained on data that skews toward temperate climates. This guide covers manual adjustments for South Florida that the algorithm may not discover on its own.

## Initial Setup Corrections

After installing your Nest, make these changes before letting it "learn":

### Turn Off Auto-Schedule (Temporarily)

1. Open Google Home app → Thermostat → Settings
2. Turn off **Auto-Schedule** for the first week
3. Manually set the schedule below
4. After 1 week, re-enable Auto-Schedule — it will learn from your corrected baseline

**Why**: If Auto-Schedule is on from day one, the Nest learns from your initial fumbling with settings and takes weeks to course-correct.

### Disable Airwave

1. Settings → Airwave
2. Turn **Off**

**Why**: Airwave shuts off the compressor early and uses the residual cold coil to finish cooling. In theory this saves energy. In practice, in South Florida's humidity, the last few minutes of "coasting" allow moisture to re-evaporate off the coil and back into your home. The energy savings (~5%) are offset by higher humidity.

### Set Temperature Differential

1. Settings → Temperature Lock → ensure no lock
2. Nest's internal differential is 1°F (not user-adjustable)
3. Acceptable for South Florida — smaller differentials are fine here

## Recommended Schedule

### Weekdays

| Time | Setpoint | Notes |
|------|---------|-------|
| 6:00 AM | 75°F | Pre-cool before wake-up (start 30 min early) |
| 8:00 AM | 78°F | Away — **not higher** to prevent humidity |
| 4:30 PM | 75°F | Pre-cool before arrival |
| 10:00 PM | 76°F | Sleep — minimal setback |

### Weekends

| Time | Setpoint | Notes |
|------|---------|-------|
| 7:00 AM | 75°F | Later wake |
| 10:00 PM | 76°F | All-day comfortable |

### Eco Temperatures (Away)

- **Cooling Eco Temp**: 78°F (default is 85°F — too high for South Florida)
- **Heating Eco Temp**: 65°F (rarely relevant)
- **Use Eco Temperatures**: When no one is home (geofencing)

> **Critical**: Change the Cooling Eco Temp from 85°F to 78°F immediately. This is the single most important change. At 85°F, your home hits 60%+ humidity in under 2 hours, creating mold conditions.

## Home/Away Assist

Nest's Home/Away Assist uses phone location and the built-in occupancy sensor.

### Recommended Settings

- **Use phone location**: Yes (for all household members)
- **Use thermostat sensor**: Yes
- **Eco Temperatures when away**: 78°F cooling (see above)
- **Home detection radius**: Leave default

### Tips

- Add all household members' phones for accurate occupancy
- If you have pets, consider raising Away temp to only 79°F
- Nest takes 2 hours of no motion to switch to Away — this is not adjustable

## Humidity Management

The Nest has limited built-in humidity control compared to Ecobee or Honeywell.

### What the Nest Can Do

- **Cool to Dry**: Runs AC below setpoint to reduce humidity (Settings → Cool to Dry)
- **Fan Timer**: Runs fan on a schedule independent of heating/cooling
- **Display humidity**: Shows current reading on the home screen

### What the Nest Cannot Do

- No humidity setpoint target
- No dehumidifier control (without separate wiring)
- No humidity-based schedule override

### Workaround: Cool to Dry

1. Settings → Cool to Dry → **On**
2. This allows Nest to cool up to 2°F below setpoint when humidity is high
3. It's automatic — no target humidity to set
4. Works reasonably well but less precise than Ecobee's approach

### Fan Timer: Use with Caution

The Nest Fan Timer runs the fan for 15 minutes per hour (adjustable). In South Florida:

- **Recommendation**: Turn it **Off**
- **If you must use it**: Set to 0 min/hr (effectively off)
- **Why**: Same reason as other brands — fan without cooling adds humidity

## Seasonal Adjustments

### Summer (May–October)

- Schedule as above
- Cool to Dry: On
- Eco temp: 78°F
- Fan timer: Off
- Filter reminder: Set to 1 month

### Winter (November–April)

- Raise daytime to 76-77°F
- Eco temp: 78°F (still relevant — South FL "winter" days can hit 85°F)
- Can enable fan timer cautiously (humidity is lower)
- Filter reminder: Set to 2 months

## Power and Wiring

### Nest Without C-Wire

The Nest can operate without a C-wire by charging its internal battery from the R and W/Y wires during heating/cooling cycles. However:

- Battery may drain if AC doesn't run enough (unlikely in South FL)
- **Symptoms of low battery**: Wi-Fi disconnects, delayed response, blank screen
- **Fix**: Add a C-wire adapter ($15-30) or repurpose the G wire (Settings → Equipment → Fan → detect wiring)

### Wiring for Heat Pump Systems

If you have a heat pump (common in newer South FL construction):

- Connect O/B wire to the O terminal
- Set O/B wire to "O" (energize on cool) — this is the Florida-standard Carrier/Trane default
- If your heat pump doesn't cool on first run, switch to "B" (energize on heat, Rheem default)

## Nest Temperature Sensor (Add-On)

Worth adding if:
- Your thermostat is in a hallway that doesn't reflect bedroom temperature
- You have a two-story home
- One room is consistently 3°F+ different from the thermostat reading

**Placement**: Same wall height as thermostat (5 feet), interior wall, away from windows and vents.
