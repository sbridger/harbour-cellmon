CellMon lets you monitor your Sailfish phones cellular radio. Install using Storeman in [Openrepos](https://openrepos.net/content/crun/cellmon)

It was started to give me a decent signal strength meter to help in finding the best signal location. 
It is also to try and help understand the loss of connection bug I experience.

- Signal strength
- 2G/3G-umts/4G-lte , band and actual frequencies (4G/lte)
- connection status

Data is read from two different apis: NetworkRegistration and NetworkMonitor
Network registration automatically updates, while NetworkMonitor is polled when you press the update button, or on a timer when the > button is active.

The Strength bars are both normalised to a 0-100 range.
Below the bars are a spinner and history so you can see when updates are happening, and catch fast changing levels.

It reads the information via dbus, and is now fairly easy to add more dbus sources

Limitation V0.2-1 support sim1/2, no detect if present.  3G frequencies probably wrong ARFCN!=EARFCN
