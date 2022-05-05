# Active Real Ring Modulator build notes

## Erratum

On the first PCB run, the transformer footprints are incorrect; mainly the problem is the dots indicating pin 1 are in the wrong place. They should look like this:

![xfrmr_ftp](../Images/xfrmr_ftp.png)

Place the dot side of the transformer toward the bottom for TR1 and toward the top for TR2.

R4 has the wrong value shown on the first run PCB silkscreen; it should be 330k, not 330R.

These were corrected after the first run.

# Build

There's nothing exotic about this build. Proceed as usual. Be careful not to overheat the germanium diodes.

Pins 2 and 3 (wiper and clockwise pins as viewed from front) of the Signal and Carrier pots should be connected together, and pins 1 and 2 should be wired to the PCB via Molex connectors or soldered directly. All three pins of the Carrier Unbalance pot should be wired to the PCB. See labels on the PCB indicating which pin goes to which point.

# Diodes

I used the rather traditional 1N695 germanium diodes but you can substitute other diodes. Regular silicon junction diodes like 1N4148 can be used although their high forward voltage means there will be more distortion. Schottky diodes like 1N5817 will have even lower forward voltage than most germanium and a steeper I vs V curve, which may give you results you'd prefer. 

Germanium diodes tend to be more variable, so if your multimeter has a diode setting, use it to select four diodes with closely matched forward voltage.
