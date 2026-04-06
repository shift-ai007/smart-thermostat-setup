# Thermostat Wiring Diagrams for South Florida Homes

Common wiring configurations found in Miami-Dade, Broward, and Palm Beach County homes, organized by system type and era.

## Standard Wire Color Reference

| Wire | Terminal | Function | Present In |
|------|----------|----------|-----------|
| Red | R (Rh/Rc) | 24V power from transformer | All systems |
| White | W (W1) | Stage 1 heat | Heat pump, gas furnace |
| Yellow | Y (Y1) | Stage 1 cooling (compressor) | All AC systems |
| Green | G | Indoor fan (blower) | All systems |
| Blue | C | Common (24V return) | Smart thermostats |
| Orange | O | Reversing valve — cool | Heat pumps (Carrier, Trane) |
| Orange | B | Reversing valve — heat | Heat pumps (Rheem, Ruud) |
| Brown/Pink | W2/Y2 | Stage 2 heat/cool | Two-stage systems |

> **Critical**: Colors are conventions, not standards. A white wire might connect to Y if the installer ran out of yellow. **Always verify at both ends** — the thermostat terminal AND the air handler terminal board.

## Configuration 1: Standard AC (Most Common)

Found in: ~70% of South Florida homes with central AC and electric heat strip

```
Thermostat          Air Handler
─────────          ───────────
R  ←── Red ──────→  R  (24V hot)
Y  ←── Yellow ───→  Y  (compressor contactor)
G  ←── Green ────→  G  (blower relay)
W  ←── White ────→  W  (heat strip relay)
C  ←── Blue ─────→  C  (24V common)
```

**Smart thermostat compatible**: Yes, if C-wire present.
**If no C-wire (4-wire system)**: R, Y, G, W only. See C-wire solutions in main README.

### 4-Wire to 5-Wire Upgrade

If your existing cable only has 4 conductors (R, Y, G, W):

**Option A — Add-a-Wire Kit:**
- Install add-a-wire module at air handler
- Module converts one existing wire to carry both its signal AND the C signal
- No new cable needed

**Option B — Run new cable:**
- Replace 18/4 cable with 18/5 (adds blue C-wire)
- Route through same path as existing cable (usually attic)
- Tape new cable to old cable and pull through

## Configuration 2: Heat Pump (Newer Construction)

Found in: Newer South Florida homes (2010+) with heat pump systems

```
Thermostat          Air Handler
─────────          ───────────
R  ←── Red ──────→  R   (24V hot)
Y  ←── Yellow ───→  Y   (compressor)
G  ←── Green ────→  G   (blower)
O  ←── Orange ───→  O   (reversing valve)
W2 ←── White ────→  W2  (aux heat strip)
C  ←── Blue ─────→  C   (common)
```

**Smart thermostat setup notes:**
- Set O/B to "O" (energize on cooling) for Carrier, Trane, Lennox, Goodman
- Set O/B to "B" (energize on heating) for Rheem, Ruud
- If unsure: try "O" first — if heat and cool seem reversed, switch to "B"
- **Aux heat lockout**: Set to 40°F in South Florida (prevents expensive heat strip use above 40°F)

## Configuration 3: Two-Stage AC

Found in: Larger South Florida homes with variable or two-stage compressors

```
Thermostat          Air Handler
─────────          ───────────
R  ←── Red ──────→  R   (24V hot)
Y1 ←── Yellow ───→  Y1  (stage 1 compressor)
Y2 ←── Pink ─────→  Y2  (stage 2 compressor)
G  ←── Green ────→  G   (blower)
W  ←── White ────→  W   (heat)
C  ←── Blue ─────→  C   (common)
```

**Notes**: Stage 1 runs at ~67% capacity (quieter, more efficient). Stage 2 engages when demand is high. Most smart thermostats support this — configure in Equipment settings.

## Configuration 4: Mini-Split (No Thermostat Wire)

Found in: Additions, condos, converted garages

Mini-splits don't use traditional thermostat wiring. They communicate between indoor and outdoor units via proprietary cables. Smart thermostat integration options:

1. **IR Blaster** (Sensibo, Cielo, Flair Puck): Mimics the remote control via infrared
2. **Wi-Fi module** (manufacturer-specific): Daikin, Mitsubishi, Fujitsu offer their own
3. **Dry contact adapter**: Some mini-splits accept a thermostat via dry contact terminals

## Troubleshooting Wiring Issues

### Thermostat Has Power But AC Won't Start

1. Check Y wire connection at air handler — loose terminal is the #1 cause
2. Verify contactor is receiving 24V (multimeter across contactor coil)
3. Check float switch — clogged condensate drain opens the safety float, breaking the circuit

### Blower Runs But No Cooling

1. Y wire may be disconnected at the air handler or condenser disconnect
2. Check outdoor unit breaker
3. Verify condenser contactor is pulling in (24V from Y wire)

### Heat Won't Turn Off

1. W wire may be shorted to R at a junction
2. Check for damaged cable in attic (rodent damage common in South Florida)
3. Verify thermostat is calling for cool (Y), not heat (W)

### Short Cycling (Turns On/Off Every Few Minutes)

1. Check for a shorted wire in the cable run
2. Verify thermostat differential isn't set too small
3. Check for refrigerant issues (low charge causes high-pressure cutout)

## Safety

- **Always turn off power at the breaker** before touching any wires
- Thermostat wires carry 24V AC — low voltage but can damage equipment if shorted
- If you see 120V or 240V wires near the thermostat location, those are NOT thermostat wires — do not connect them
- When in doubt, photograph everything and consult a licensed HVAC technician
