# DC Power on a Boat

This document summarises options for DC power on a Boat.


# Inputs

The following inputs may be available

Shore AC - 240V

Engine Alternator / Starter Battery

Solar

Wind


### Shore AC

Shore AC needs converting to DC with a battery charger. Multiple battery chargers can work together. The battery charger must be compatible with the type of battery in use.

### Engine Alternator

The engine alternator charges a starter battery.
A voltage dependent relay should be used to connect the starter battery to the leisure battery. This way the leisure battery will only be charged from the alternator when the starter battery is above a set voltage.

### Solar
Solar panels must go through a solar battery controller. Multiple battery controllers can be connected in parralel. 

### Wind
AFAIK this works the same as Solar, but further research required.



# Battery Controllers

When in use with Lead Acid Batteries, A controller must have a temperature sensor which is connected to the battery bank. The controller also needs to be compatible with the type of battery, and may need programming for the initial setup.

## PWM
PWM controllers are cheap upfront but less efficient then MPPT controllers. They also have a lower maximum voltage. This means that if multiple solar panels are being used, they must be connected in parrallel, and so the gauge of the copper wires must be larger / more expensive.
It can howerver still be cheaper to have multiple PWM Controllers, with one for each solar panel.
The efficiency is roughly 70% to 90% of a MPPT controller.
Until you run out of space, it is usually more efficient to buy more solar panels the buy a better controller.

## MPPT
MPPT has advantages in that the solar panels can be connected in series, as they allow a much larger input voltage. This decreases the price of the copper wiring.
MPPT is more efficient in the conversion.



# Power monitors
The Victron Energy Monitors look the best - with the Inline Shunts (Without the Monitor)[https://www.victronenergy.com/battery-monitors/smart-battery-shunt] or (With the monitor)[https://www.victronenergy.com/battery-monitors/bmv-712-smart]. 

Much Cheaper Dumb monitors also exist.

Smarter solar battery monitors also exist. This will allow monitoring of the specific inputs. Victron appears the only relavivly cheap ecosystem that allows integration of all of these devices. This is not cheap.


# Wireing


# Upgrade path.

### Current system

Alternator charges the starter battery (With a voltage dependant split relay?)


### Solar power initial upgrade

Add a Single solar panel with a pwm controller


### Solar power upgrade 2

Depending on cost of copper wire vs cost of the controller, add a second solar panel in series or upgrade the controller to a MPPT controller.


### Shore Power upgrade

Wire the current solution in, but better.


### Change battery technology

Lithium Batteries last decades instead of years. This should be considered.

### Add monitoring
Get a victron smart monitor (With optional display) to see what idle power use is, and what nightly power use is like.

### Upgrade the fuse box
The current fuse box is too small. Upgrade this.

### Add a new bus bar
The new bus bar should have inputs from the alternator, the solar battery controller, the battery, the fuse box, and the shore power.


# Voltage

### 12V
12V is the standard output and should most likely stay this way.

However, if using more then a couple of batteries, storing charge at 24V with DC-DC converters allows faster charging and cheaper solar controllers to be used as they are usually current limited instead of power limited.



