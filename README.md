# `prt_sim` - Precomputed Radiance Transfer Helper

`prt_sim` is a helper tool that calculates [PRT lighting](https://learn.microsoft.com/en-us/windows/win32/direct3d9/precomputed-radiance-transfer) for an input rigid single material mesh, compresses the result and saves it out to disk for further processing by tool. PRT allows for better lighting for complex objects including self shadowing.

![Comparison of a PRT enabled evalator model vs a non PRT enabled model on moonbase](prt_comparison.png)

# Instalation

1. Download the [latest version from releases](https://github.com/digsite/prt_sim/releases)
2. Copy the executable to the H2EK root directory
3. You may need to install the DirectX redist package provided, if you haven't already installed the latest DirectX End-User Runtimes (June 2010) bundle.

# Usage

You can generate a PRT compatible render model by importing it with the prt flag set.

```
tool render objects/your/tag/goes/here 0 1
```

For an existing PRT enabled render model you can re-run the PRT simulation using:

```
tool prt-simulation scenarios\objects\multi\zanzibar\main_crane\main_crane
```

# Disclaimer

**THIS SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.***

# LICENSE
Note that this project is ***not*** open source. You are not granted any rights to use this content commercially, or for any projects outside of Halo: The Master Chief Collection. Please read the MCC EULA, MCC EULA FAQ, and Xbox EULA for additional information and context.

As a courtesy pointing to this reprository instead of rehosting `prt_sim` is preferred when possible, as this ensures users can access the latest version of the tool.

## EULA
* https://www.halowaypoint.com/halo-the-master-chief-collection/eula
* https://www.halowaypoint.com/news/mccs-eula-the-faq
* https://www.xbox.com/en-us/developers/rules

# Issues

Please report issues in this reprository, included the .msb file and command line options used in all bug reports. You may be asked to share a minimal set of tags for reproducing visual bugs.

