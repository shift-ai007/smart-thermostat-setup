# Honeywell Home T9 — Dehumidification Setup for South Florida

The Honeywell T9 has the best built-in dehumidification controls of any mainstream smart thermostat. This guide covers optimal configuration for South Florida's high-humidity environment.

## Why the T9 Excels at Humidity

Unlike Nest (which only has "Cool to Dry" toggle) and Ecobee (overcool only), the T9 offers a dedicated **Dehumidify** mode that can:

- Run AC in a dehumidification cycle independent of cooling demand
- Control fan speed to maximize moisture removal
- Set a specific humidity target (not just an overcool offset)
- Coordinate with whole-home dehumidifiers via equipment interface

## Step-by-Step Configuration

### 1. Set Humidity Target

1. Open Honeywell Home app → select T9 thermostat
2. Tap **Indoor Humidity** reading (bottom of screen)
3. Set target: **50%**
4. Enable **Auto Dehumidify**

**Why 50% and not 45%**: The T9's dehumidification is aggressive enough that setting to 45% can cause excessive runtime. Start at 50%, monitor for two weeks, then lower to 48% or 45% if your home still feels humid.

### 2. Configure Dehumidification Behavior

Settings → Equipment → Dehumidification:

| Setting | Value | Notes |
|---------|-------|-------|
| Dehumidification Mode | Auto | Activates when humidity exceeds target |
| Dehumidify Using | AC + Fan Speed | Most effective method |
| Max Overcool | 2°F | Prevents over-cooling |
| Min Cool Duration | 8 minutes | Ensures coil gets cold enough to condense |

### 3. Fan Settings

Settings → Equipment → Fan:

| Setting | Value | Reason |
|---------|-------|--------|
| Fan Circulate | Off | Prevents re-evaporation |
| Fan Off Delay | 60 seconds | Short post-cooling run |
| Fan During Dehumidify | Low speed | Slower air = more moisture removal |

**The key insight**: During dehumidification, slow fan speed keeps air in contact with the cold evaporator coil longer, extracting more moisture per minute. The T9 is one of the few thermostats that can control this.

### 4. Schedule Template

Program → Schedule:

**Weekdays:**

| Time | Cool Setpoint | Humidity Target |
|------|-------------|----------------|
| 6:00 AM | 75°F | 50% |
| 8:30 AM | 78°F | 50% |
| 5:00 PM | 75°F | 48% |
| 10:00 PM | 76°F | 50% |

**Weekends:**

| Time | Cool Setpoint | Humidity Target |
|------|-------------|----------------|
| 7:00 AM | 75°F | 50% |
| 10:00 PM | 76°F | 50% |

### 5. Geofencing

Settings → Geofence:

- Enable for all household phones
- **Away cooling**: 78°F (change from default 85°F)
- **Away humidity**: 50% (humidity control stays active even in away mode)
- **Arrival pre-cool**: 30 minutes

## Room Sensor Placement

The T9 includes one room sensor. Best placement for South Florida humidity monitoring:

### Priority Locations (Pick One)

1. **Master bedroom** — comfort during sleep, furthest from AC in many floor plans
2. **Home office** — where you spend most indoor time
3. **Problem room** — any room with history of musty smell or mold

### Placement Rules

- Mount at 5 feet on an interior wall
- At least 3 feet from any vent (supply or return)
- Away from windows, exterior doors, and appliances that generate heat
- Not in direct sunlight path
- Not in the kitchen or bathroom (temporary spikes)

### Using the Sensor for Scheduling

- **Day**: Use thermostat sensor (central location where you want consistent temp)
- **Night**: Use bedroom sensor (optimize for sleep comfort)
- Configure in: Settings → Room Sensors → Room Priority

## Monitoring and Adjustment

### First Two Weeks

After configuration, monitor:

1. **Humidity readings**: Should stay between 45-52% most of the time
2. **AC runtime**: Will increase slightly compared to cooling-only mode — this is normal
3. **Energy use**: Expect 5-10% increase in electricity during summer months
4. **Comfort**: Home should feel noticeably less clammy

### Signs You Need to Adjust

| Symptom | Fix |
|---------|-----|
| Humidity stays above 55% | Lower target to 48%, check if AC is right-sized |
| Home feels too cold | Increase max overcool to only 1°F |
| AC runs constantly | Raise target to 52%, check filter and coil |
| Condensation on windows | Lower target to 45%, check for air leaks |

### Seasonal Adjustments

**Summer (June-September)**: Keep all dehumidification settings aggressive. This is when you need them most.

**Shoulder months (October, April-May)**: Humidity can be high even when cooling demand is low. The T9's independent dehumidification mode is most valuable here — it runs the AC specifically to dehumidify without over-cooling.

**Winter (November-March)**: Can raise humidity target to 52-55%. South Florida's winter humidity is lower but still above national norms.

## Whole-Home Dehumidifier Integration

If your HVAC system includes a whole-home dehumidifier (Aprilaire, Santa Fe, Ultra-Aire):

1. Connect dehumidifier wires to T9's DHM terminal
2. Settings → Equipment → Dehumidifier → Enable
3. Set priority: **Dehumidifier first, AC second**
4. This saves significant energy — dedicated dehumidifiers use 40-60% less electricity than using the AC to dehumidify

## Troubleshooting

### "Aux Heat" Appears on Screen
- You may have wired auxiliary heat to the W2 terminal
- In South Florida this rarely activates (only below 40°F)
- If it runs during summer, wiring may be crossed — call a technician

### App Shows Different Humidity Than Thermostat
- Normal — app updates every 5 minutes, thermostat is real-time
- Sensor readings may also differ from thermostat (different locations)
- Use the higher reading as your reference

### Thermostat Clicks but AC Doesn't Start
- 5-minute compressor delay is normal after a shutoff (protects compressor)
- If longer than 5 minutes, check the outdoor unit breaker
- Verify the contactor is engaging (audible click at the outdoor unit)
