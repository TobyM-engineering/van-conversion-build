# Wiring System

This section explains how the van electrical wiring is organized and how power moves through the system.

<p align="center">
  <img src="photos/battery-inverter%20%282%29.jpg" width="300">
  <img src="photos/fuse-box-wiring.jpg" width="300">
  <img src="photos/control-panel.jpg" width="300">
</p>

<p align="center">
  <b>Battery + Inverter</b> &nbsp;&nbsp;&nbsp; <b>Fuse Box + Wiring</b> &nbsp;&nbsp;&nbsp; <b>Control Panel</b>
</p>

## System Overview

The van uses a 12V house battery as the main power source. Power is distributed from the battery to the inverter, fuse panel, control switches, lights, fridge, water pump, outlets, and accessories.

The system is split into two main parts:

- **12V DC power** for lights, fridge, water pump, switches, and accessories
- **120V AC power** from the inverter for standard wall-style outlets

## Power Flow

Power starts at the LiFePO4 house battery. The main positive line is protected with fusing before power is distributed to the rest of the van.

Basic DC power path:

```txt
Battery
  → Main fuse protection
  → DC fuse/control panel
  → Switches and protected circuits
  → Lights, pump, fridge, outlets, and accessories
````

Basic AC power path:

```txt
Battery
  → 3000W inverter
  → AC outlets
```

The inverter converts 12V battery power into standard AC power so normal plug-in devices can be used inside the van.

## Charging Wiring

The battery can be charged from solar power or shore power.

<p align="center">
  <img src="photos/solar-charge-controller.jpg" width="300">
  <img src="photos/shore-power-charger.jpg" width="300">
</p>

<p align="center">
  <b>Solar Charge Controller</b> &nbsp;&nbsp;&nbsp; <b>Shore Power Charger</b>
</p>

The solar panels feed into the solar charge controller, which regulates the charging voltage and current going into the battery.

The shore charger allows the van battery to be charged from a standard house outlet when the van is parked.

Solar charging path:

```txt
Solar Panels
  → Solar Charge Controller
  → House Battery
```

Shore charging path:

```txt
House Outlet
  → Shore Charger
  → House Battery
```

## Fuse and Control Panel

The fuse panel protects each smaller circuit in the van. Instead of running every device directly from the battery, each load has its own protected path.

This makes the system safer and easier to troubleshoot because a problem with one circuit does not shut down the entire van.

Examples of fused circuits:

* Interior lights
* Exterior lights
* Water pump
* Fridge
* DC outlets
* Accessory switches
* Control panel power

## Switch Wiring

The control panel is used to turn different loads on and off from one central location. Power runs from the fuse panel to the switches, then from each switch to the device it controls.

Example switch path:

```txt
Battery
  → Fuse Panel
  → Switch
  → Light / Pump / Accessory
```

This keeps the wiring organized and makes the van easier to use.

## Ground / Negative Wiring

Each device needs a complete circuit, so the negative wires return back to the battery negative side or a shared negative bus.

The positive side is fused and switched. The negative side completes the return path back to the battery.

## Design Goals

The wiring layout was built around:

* Safe power distribution
* Protected circuits
* Clean wire routing
* Easy access for repairs
* Separate AC and DC systems
* Reliable charging from solar or shore power
* Enough power for real use inside the van
