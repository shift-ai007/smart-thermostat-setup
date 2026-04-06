# Smart Thermostat Setup Guide for Humid Climates

Everything you need to know about choosing, installing, and configuring smart thermostats in high-humidity environments like South Florida. Default factory settings are optimized for moderate climates — this guide covers the adjustments that actually save money and prevent mold in subtropical heat.

> Maintained by [AC Repair Today](https://ac-repair.today) — Licensed Florida HVAC Contractor (CAC1824118)

## Why Default Settings Fail in South Florida

Smart thermostats promise 10-15% energy savings, but those numbers come from Department of Energy studies conducted in temperate climates. In South Florida's heat and humidity, default settings cause three common problems:

1. **Humidity creep** — Default target of 60% RH is too high. Above 55%, mold growth accelerates on walls, in ducts, and behind furniture
2. **Aggressive setbacks** — An 8-10°F night setback that works in Denver creates a humidity spike in Miami that takes hours to recover from
3. **Away mode too high** — Setting to 85°F while at work allows humidity to climb above 65%, creating conditions for mold in just 24 hours

The fix isn't complicated — it's just different from what the manual says.

## Thermostat Comparison

| Feature | Ecobee Premium | Google Nest Learning | Honeywell T9 | Honeywell T6 Pro |
|---------|---------------|---------------------|--------------|-----------------|
| **Price** | $250 | $250 | $200 | $120 |
| **Remote Sensors** | 1 included | Sold separately ($40) | 1 included | None |
| **Humidity Control** | Good | Basic | Best | Good |
| **Dehumidify Mode** | AC overcool | Fan timer only | Dedicated mode | AC overcool |
| **C-Wire Required** | Yes (adapter included) | No | Yes | Yes |
| **Geofencing** | Yes | Yes (excellent) | Yes | No |
| **Voice Assistant** | Alexa built-in | Google built-in | Both via app | Both via app |
| **Best For** | Large homes with hot spots | Tech-savvy, set-and-forget | Humidity priority homes | Budget, straightforward |

### Our Recommendation for South Florida

**Best overall**: Honeywell T9 — best humidity control, remote sensors included, no-nonsense interface.

**Best for tech enthusiasts**: Google Nest Learning — excellent geofencing and learning algorithms, but humidity management requires manual configuration.

**Best for large homes**: Ecobee Premium — remote sensors detect hot spots and redirect cooling where needed.

## Installation

### Before You Start

1. **Turn off power** at the breaker (not just the thermostat)
2. **Photograph your current wiring** before disconnecting anything
3. **Label each wire** with the terminal it's connected to (R, W, Y, G, C, etc.)
4. **Check for a C-wire** — it provides constant 24V power to the thermostat

### C-Wire Solutions for Older Homes

Most South Florida homes built before 1995 lack a C-wire (common wire). Your options:

#### Option 1: Ecobee Power Extender Kit (Easiest)
- Included free with every Ecobee thermostat
- Installs at the air handler, no new wire needed
- Works with most single-stage and two-stage systems
- **Not compatible** with: heat pumps with auxiliary heat strips using W2

#### Option 2: Add-a-Wire Adapter ($15–$30)
- Converts your existing 4-wire cable to carry a C-wire signal
- Brand: Fast-Stat Common Maker or Venstar Add-a-Wire
- Installs in 15 minutes at the air handler
- Works with Nest, Honeywell, and most other brands

#### Option 3: Repurpose the G-Wire (Nest Only)
- Google Nest can power itself from the G (fan) wire
- Trade-off: fan always runs with cooling (no independent fan mode)
- Acceptable in South Florida where independent fan mode increases humidity anyway

#### Option 4: Run New Thermostat Wire (Professional)
- Required for complex systems (multi-stage, heat pump with aux)
- 18/5 or 18/8 thermostat wire through attic or wall
- Cost: $150–$300 professional installation
- Worth it if you're also replacing the thermostat during an AC upgrade

### Wiring Reference

Standard residential HVAC wire colors:

| Wire Color | Terminal | Function |
|-----------|----------|----------|
| Red | R (Rh/Rc) | 24V power |
| White | W | Heat (or W1/W2 for stages) |
| Yellow | Y | Cooling (compressor) |
| Green | G | Fan |
| Blue | C | Common (24V return) |
| Orange | O/B | Heat pump reversing valve |
| Brown | varies | Auxiliary/emergency heat |

> **Warning**: Wire colors are conventions, not standards. Always verify by tracing each wire to the air handler control board. The terminal letter matters, not the color.

## Configuration for South Florida

These settings are the core of this guide. Apply them after installation.

### Humidity Control (Critical)

| Setting | Factory Default | South Florida Setting |
|---------|----------------|---------------------|
| Target humidity | 55–60% | **45–50%** |
| Humidity alert | Off or 65% | **55%** |
| Overcool to dehumidify | Off | **On, max 2°F** |
| Fan after cooling | Off | **Off** (running fan re-evaporates moisture) |
| Fan schedule | Circulate 15 min/hr | **Off** (adds humidity in shoulder seasons) |

**Why "Fan: Circulate" is bad in South Florida**: In dry climates, circulating air helps distribute temperatures. In South Florida, running the fan without cooling blows humid air across the wet evaporator coil, re-evaporating condensed moisture back into your home. This can add 5-10% RH.

### Schedule Settings

| Time Block | Recommended Setpoint | Notes |
|-----------|---------------------|-------|
| **Morning** (6-8 AM) | 75°F | Comfortable wake-up |
| **Day/Away** (8 AM-4 PM) | 78°F | Max 78° to prevent humidity spike |
| **Pre-cool** (4-5 PM) | 75°F | Cool before peak demand pricing |
| **Evening** (5-10 PM) | 75°F | Active hours comfort |
| **Sleep** (10 PM-6 AM) | 76-77°F | Only 1-2° setback, not 8-10° |

**Critical: Never set Away above 80°F in South Florida.** National energy guides recommend 85°F for away mode. In South Florida humidity, 85°F allows indoor RH to climb above 60% within 2 hours. Above 60% RH, mold begins growing on drywall, wood, and fabrics within 24-48 hours.

### Geofencing Settings

- **Home radius**: 2 miles (South Florida traffic means you could be "close" for 30+ minutes)
- **Away delay**: 30 minutes (prevents away trigger for quick errands)
- **Away setpoint**: 78°F (not 85°F — see humidity warning above)
- **Pre-cooling lead time**: 30 minutes before arrival

### Multi-Zone Homes

If your home has 2+ zones:
- **Upstairs zone**: Set 1-2°F cooler than downstairs (heat rises)
- **Guest room zone**: Never fully shut off — minimum 80°F to prevent musty odors
- **Use remote sensors** to measure actual occupancy temperatures, not just hallway reading

## Troubleshooting

### AC Won't Stop Running
- Check that temperature differential isn't set too small (less than 1°F causes rapid cycling)
- Verify overcool-to-dehumidify isn't set above 3°F
- If outdoor temp is above 95°F, your AC may legitimately need to run continuously

### Humidity Stays High Despite AC Running
- **Check fan setting**: Must be "Auto" not "On" or "Circulate"
- **Check filter**: A dirty filter reduces coil contact time, reducing dehumidification
- **Check sizing**: An oversized AC cools too quickly and shuts off before removing humidity (short cycling)
- **Check ductwork**: Leaky supply ducts in the attic pull humid outside air into the system

### Thermostat Shows Wrong Temperature
- Remote sensors override the thermostat's built-in sensor — check which sensor is active
- Direct sunlight on the thermostat adds 3-5°F ghost reading
- Mounting on an exterior wall transfers heat through the drywall

### Wi-Fi Drops
- Ensure thermostat is within router range (interior walls reduce signal)
- Metal ductwork near the thermostat can block Wi-Fi
- Use 2.4 GHz network (better range than 5 GHz)

## Energy Savings Expectations

Realistic savings for South Florida, not manufacturer marketing numbers:

| Scenario | Expected Annual Savings |
|----------|----------------------|
| Replacing a manual thermostat with programmed schedule | $150–$300 |
| Adding geofencing (irregular schedule household) | $100–$200 |
| Optimizing humidity settings (reducing overcooling) | $50–$100 |
| Remote sensors (reducing hot-spot overcooling) | $50–$150 |
| **Total realistic savings** | **$200–$500/year** |

Savings assume a typical 2,000 sq ft South Florida home with a 3-ton AC system and current FPL rates.

## Additional Resources

- [`docs/ecobee-humidity-settings.md`](docs/ecobee-humidity-settings.md) — Step-by-step Ecobee humidity configuration
- [`docs/nest-schedule-optimizer.md`](docs/nest-schedule-optimizer.md) — Optimal Nest schedules for South Florida
- [`docs/honeywell-t9-dehumidify.md`](docs/honeywell-t9-dehumidify.md) — Honeywell T9 dehumidification setup
- [`docs/wiring-diagrams.md`](docs/wiring-diagrams.md) — Common thermostat wiring configurations for South FL homes

## Contributing

Found something inaccurate or have a tip for a specific thermostat model? Open an issue or PR. We especially value feedback from South Florida HVAC technicians and homeowners with real-world experience.

## License

MIT License — see [LICENSE](LICENSE) for details.

---

*This guide is maintained by [AC Repair Today](https://ac-repair.today) — your licensed South Florida HVAC contractor. For professional thermostat installation including C-wire solutions, call (800) 917-2580.*
