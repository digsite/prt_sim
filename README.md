# `prt_sim` - Precomputed Radiance Transfer Helper

`prt_sim` is a helper tool that calculates [PRT lighting](https://learn.microsoft.com/en-us/windows/win32/direct3d9/precomputed-radiance-transfer) for an input rigid single material mesh, compresses the result and saves it out to disk for further processing by tool. PRT allows for better lighting for complex objects including self shadowing.

# Instalation

1. Download the [latest version from releases](https://github.com/digsite/prt_sim/releases)
2. Copy the executable to the H2EK root directory
3. You may need to install the DirectX Redistributable provided, if you haven't already installed the latest DirectX End-User Runtimes (June 2010) bundle.

# Usage

You can generate a PRT compatible render model by importing it with the prt flag set.

```
tool render objects/your/tag/goes/here 0 1
```

For an existing PRT enabled render model you can re-run the PRT simulation using:

```
tool prt-simulation scenarios\objects\multi\zanzibar\main_crane\main_crane
```

# LICENSE
Note that this project is ***not*** open source. You are not granted any rights to use this content commercially, or for any projects outside of Halo: The Master Chief Collection. Please read the MCC EULA, MCC EULA FAQ, and Xbox EULA for additional information and context.

## EULA
* https://www.halowaypoint.com/halo-the-master-chief-collection/eula
* https://www.halowaypoint.com/news/mccs-eula-the-faq
* https://www.xbox.com/en-us/developers/rules

# Issues

Please report issues in this reprository, included the .msb file and command line options used in all bug reports. You may be asked to share a minimal set of tags for reproducing visual bugs.

