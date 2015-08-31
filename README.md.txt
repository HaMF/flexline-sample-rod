# Flexline sample rod

This sample rod was designed to allow magnetic resonance experiments and simulateneous measurements in a Bruker flexline MD5 resonator hold inside of a Oxford CF395 flow cryostat. Included are 3d-models, drawings, PCB layouts and production recommendations as well as part lists of stock ISO KF parts.

All in all the holder works quite nicely. It positions the sample quite accurately in the cavity's center, is leak tight, does not show performance degradation or extraordinary large heat conductions at low temperatures (liquid Helium). Empty cavity measurements vs. sample holder in cavity measurements have been performed and will be added here for reference when the results are polished. A gear can be fitted to the top rod and the whole rod can be rotated automatically (http://hannes.maier-flaig.de/goniometer/)

**Please note:** Initial design documents were in German and some elements will probably have slipped through when translating to english (read: _all_ drawings). Units are exclusively metric. 3D models of of-shelf ISO-KF flange parts (as available from the vendors web site) are included in the project. No copyright infrigement intended.


## Pictures and performance

The full construction as autodesk project can be found in the subfolder ./1-autodesk project/ . Drawings are also exported
to PDF in the ./2-drawings folder. Here follows a description of the parts and description of the PCB holders:

### Top
Standard ISO-KF flanges are used. Conical reduction piece [Fig. ... (2)] is beneficial because it has more space to fit the connector.
Connecting the DC lines to a breakout box is performed using lemo connectors.

### V2A rod
To the lower KF16 KF a V2A rod is welded (i.e. hard soldered).

### Sample holder support
The sample rod is designed so that Bruker holder for standard quartz glass sample tubes also fit.
In this case an extension [Fig. ... (1)] has to be used that fits the plug of the DC lines.

Shown in [Fig. ... (2) and Fig ...] is the sample holder support for PCB sample holders.

## PCB sample holders
The PCB design in ./3-PCB/PCB.brd and ./3-PCB/PCB.pdf includes three layers: Dimensions, Holes, and Top (Copper)).
It was produced on FR4 IT158 (Tg155) 1mm thickness with a cooper only plating of 35µm. All of that is pretty standard
With the supplier "Hofmann Leiterplatten" production was fast and troublefree. After tax cost was roughly 190€ per 50pcs.

 + Soldering PCBs using a hotplate and soldering paste works quite nicely. Trim pins that stick out to the backside first.
 + When breaking PCB free from full plate, length dimensions are slightly too long thus the PCBs need to be shortened. (See below)

## Empty cavity vs loaded cavity measurements

Will follow.


# Part list

| Part # | Manufacturer          | Model               | Description                                                                        |
|--------|-----------------------|---------------------|------------------------------------------------------------------------------------|
| 1      | Lemo                  | HGP.1S.306.CLLSV    | 6-pin vacuum tight receptangle                                                     |
| 2      | Pfeiffer Vacuum       |                     | ISO KF-40 blind flange (Al)                                                        |
| 3      | Pfeiffer Vacuum       |                     | ISO KF-40 centering ring and o-ring                                                |
| 4      | Pfeiffer Vacuum       |                     | ISO KF-40-16 conical reduction (Al)                                                |
| 5      | Pfeiffer Vacuum       |                     | ISO KF-16 centering ring and o-ring                                                |
| 6      | Pfeiffer Vacuum       |                     | ISO KF-16 blind flange (Al)                                                        |
| 7      |                       |                     | V2A tube, 8mm OD, 7mm ID                                                           |
| 8      |                       |                     | PEEK-1000 rod, 10mm OD                                                             |
| 9      | W+P Products          | 605-006-1-2-00      | Plug 1.27mm grid, 2 rows each 3 pins at Conrad electronics: 739179-05              |
| 10     | W+P Products          | 712-1-006-2-10-00   | Plug 1.27mm grid, 2 rows each 3 pins, right angle at Conrad electronics: 718818-05 |
| 11     | Hofmann Leiterplatten |                     | PCB sample holder, see below                                                       |
| 12     | Lemo                  | 060080              | Cable for in-road as well as to breakout box                                       |
| 13     | Lemo                  | FFA.1S.306.CLAC52ZN | Plug, straight for breakout box. 2 times                                           |
| 14     | Lemo                  | ERA.1S.306.CLL      | Receptangle for breakout box                                                       |
| 15     | Telegärtner           | J01001A0043         | Isolating BNC female, straight for breakout box                                    |

## Remarks on parts, design considerations
 +  Sample side plug and jack are not polarity proof. This would be possible e.g. with Omnetics miniature plugs. 
    These are, however too expensive for this type of application and are not justified by just being polarity proof


# Further plans (and decisions that turned out not to be so clever)

 + Even though there are 6 DC lines, the PCBs connect only 5 into the cavity. Six leads would fit on the PCB just as well. 
   In case very low loading of the cavity is needed, only two leads should be used in any case.
 + PCB with 1.27x2.54mm² grid dimensions use 1.27x1.27mm² in next iterations. Rod-side is already the later gridsize.
 + PCB tolerance when breaking free instead of milling has been choosen too small. PCBs should be 0.5mm shorter in next iteration






