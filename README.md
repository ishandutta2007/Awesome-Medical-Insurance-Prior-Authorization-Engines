# Awesome-Medical-Insurance-Prior-Authorization-Engines

## Top Microchip Thermal Layout Architecture Engines Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Thermal-Aware Floorplanning, Electro-Thermal Co-Simulation & Hot-Spot Prevention*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Microchip Thermal Layout Architecture Engines**. These tools help chip designers analyze heat build-up across complex processor architectures, optimize floorplans to avoid thermal hotspots, and co-simulate electrical and thermal behavior — enabling faster, cooler, and longer-lasting chips.

**Examples** include Ansys Icepak, Cadence Celsius, Siemens Simcenter Flotherm, Synopsys, Celestial AI, Arteris, Silvaco, Movellus, ProteanTecs, and Enosemi (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, open-source EDA flows, and transparent thermal simulation — ideal for chip designers prioritizing accessibility, academic researchers building novel architectures, and teams avoiding expensive commercial licenses.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Ansys Icepak](https://www.ansys.com/products/electronics/ansys-icepak)**  
  Industry-standard electronics cooling simulation tool for component, board, and system-level thermal analysis. Widely used for chip package and PCB thermal management.

- **[Cadence Celsius](https://www.cadence.com/)**  
  Thermal and electro-thermal simulation platform integrated with Cadence's digital and analog design flows. Provides 3D thermal analysis from chip to system level.

- **[Siemens Simcenter Flotherm](https://www.plm.automation.siemens.com/global/en/products/simcenter/flotherm.html)**  
  Leading CFD-based thermal simulation software for electronics cooling. Standard tool for chip package and system-level thermal analysis in commercial design flows.

- **[Synopsys](https://www.synopsys.com/)**  
  EDA platform with thermal-aware physical design, power integrity, and electro-thermal analysis integrated into the digital implementation flow.

- **[Celestial AI](https://celestial.ai/)**  
  Photonic fabric technology for AI compute with thermal-aware chiplet architectures.

- **[Arteris](https://www.arteris.com/)**  
  Network-on-chip (NoC) IP with thermal-aware interconnect design for heterogeneous SoCs.

- **[Silvaco](https://www.silvaco.com/)**  
  TCAD and EDA tools with thermal simulation and electro-thermal analysis for semiconductor devices.

- **[Movellus](https://www.movellus.com/)**  
  Clock generation and power management IP with thermal-aware design capabilities.

- **[ProteanTecs](https://www.proteantecs.com/)**  
  Deep data analytics for electronics health and performance monitoring including thermal profiling.

- **[Enosemi](https://www.enosemi.com/)**  
  Chip design services and tools with thermal-aware physical design.

## Open-Source GitHub Projects

- **[TASChips](https://www.nsf.gov/cise/updates/nsf-funded-tool-helps-chips-run-faster-cooler-longer)**  
  **NSF-funded open-source thermal analysis tool** from Clarkson University. Predicts in real time how heat builds up inside advanced processors. Merges **physics-based models with reduced-order learning algorithms** to identify thermal hot spots across complex chip architectures. Designed to simulate even the largest processors with 100,000+ cores — where older tools either run fast but miss details or deliver accurate results too slowly [citation:6][citation:11]. Will be released on GitHub with documentation and case studies. Funded by a three-year, $597,316 NSF grant [citation:17].

- **[Corblivar](https://archive.softwareheritage.org/browse/content/sha1_git:55dd6fb72e9343000de74e128e321d3f4fee4b70/raw/)**  
  **Open-source thermal-aware floorplanner for 3D ICs.** Performs thermal analysis using Octave scripts for parameterization of power-blurring-based thermal analysis. Integrates with BU's **3D HotSpot** thermal simulator. Features system-level static timing analysis, analysis and mitigation of **thermal side-channel (TSC)**, voltage assignment, and TSV (through-silicon via) handling with dummy TSV grid insertion [citation:2]. Uses MCNC, GSRC, and IBM-HB+ benchmarks. Gnuplot scripts for generating thermal maps and floorplan visualizations.

- **[Open3DFlow](https://doaj.org/article/2cd77978b7074b3799cbc96de55f73d8)**  
  **Open-source design platform for 3D ICs with integrated thermal analysis.** Seven-step workflow incorporating essential ASIC back-end processes with support for multi-physics analysis including **through-silicon via (TSV) modeling, thermal analysis, and signal integrity (SI) evaluations**. Demonstrated with a 3D RISC-V CPU design with vertically stacked L2 cache on separated die, hardened in GlobalFoundries 180nm (GF180) process with open-source PDK support. Enables face-to-face (F2F) die coupling by constructing a bonding layer. Open-source nature allows integration of custom AI optimization algorithms including LLM-assisted bonding pad placement [citation:12].

- **[OpenROAD](https://theopenroadproject.org/)**  
  **Foundational open-source VLSI design application from RTL to GDSII.** While primarily a physical design tool, it provides the infrastructure for thermal-aware design flows. The **PDNSim** module performs power grid analysis including IR drop and electromigration, which are critical inputs for thermal analysis [citation:4][citation:18]. Used by OpenFASoC for automated analog/mixed-signal generation including temperature sensor and LDO generators. OpenROAD's Python/Tcl API allows fine-grained control over floorplanning and power component placement for thermal optimization [citation:4].

- **[OpenFASoC](https://github.com/alibillalhammoud/OpenFASOC)**  
  **Fully open-source autonomous SoC synthesis using customizable cell-based synthesizable analog circuits.** Built on top of OpenROAD. Includes **temperature sensor** and **low dropout voltage regulator (LDO)** generators for SKY130 and GF180 nodes [citation:9]. The LDO design includes "highly trimmable voltage references to address dependencies on or sensitivities to **temperature variation**" [citation:4]. Uses Magic, Netgen, KLayout, Yosys, OpenROAD, open_pdks, and Xyce in a complete open-source flow.

- **[Open-PDKs](https://github.com/openfnord/open_pdks)**  
  **Open-source Process Design Kit installer for open-source EDA tools.** Provides SkyWater SKY130 130nm and GlobalFoundries GF180MCU PDKs with thermal-relevant device models and technology files [citation:5][citation:10]. Required for running thermal and electro-thermal simulations with open-source tools. Apache 2.0 licensed.

- **[Elmer FEM](http://www.elmerfem.org/)**  
  **Open-source multiphysics simulation software including 2D/3D heat conduction** (steady-state and optional transient) with package and boundary condition support. Used in open-source RFIC design flows for **thermal/electro-thermal co-simulation** — deriving power density from circuit simulation, thermally simulating selected sub-structures, and back-annotating resulting temperatures into circuit/EM simulation for system-level performance impact [citation:1].

- **[openEMS](https://openems.de/)**  
  **Open-source FDTD (Finite-Difference Time-Domain) electromagnetic field solver** with thermal co-simulation capabilities. Used alongside KLayout/gdsfactory for layout and EM analysis in open-source chip design flows [citation:1].

- **[KLayout](https://www.klayout.de/)**  
  **Open-source layout viewer and editor with scripting support** for parametric cell generation and thermal-aware layout analysis. Used in open-source design flows for floorplanning and integration with thermal simulation tools [citation:1].

- **[gdsfactory](https://gdsfactory.github.io/gdsfactory/)**  
  **Python library for generating GDSII layouts with parametric PCells.** Enables programmatic floorplan generation and integration with thermal analysis workflows [citation:1].

### Additional Strong Open-Source Options

- **iEDA** — Open-source intelligent physical implementation toolkit covering floorplan, placement, CTS, routing, timing optimization, and analysis tools including Static Timing Analysis and Power Analysis. Taped out three chips (700k-1.5M gates) on 110nm and 28nm nodes [citation:13].
- **DI-PASSIONATE** — German BMFTR-funded project creating open-source design and simulation environment for 2.5D/3D chip systems with 3D modeling, electrical, and thermal simulation. Extends existing tools for heterogeneous chiplet integration [citation:7].
- **Chipyard** — Open-source RISC-V SoC design framework from UC Berkeley with Hammer VLSI flow for place-and-route and thermal-aware physical design [citation:3][citation:14].
- **HotSpot** — Thermal modeling tool for microprocessors (often paired with Corblivar for 3D IC thermal analysis).
- **ThermOS** — Open-source thermal simulator from UMN-EDA [citation:18].

**Frameworks for building custom systems**: Combine **TASChips** for real-time thermal hot-spot identification with reduced-order learning, **Corblivar** for thermal-aware 3D floorplanning, **Open3DFlow** for 3D IC design with integrated TSV and thermal analysis, **OpenFASoC** for temperature-aware analog generation, and **Elmer FEM** for electro-thermal co-simulation to build a complete open-source microchip thermal layout stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Microchip thermal analysis tools must be validated against foundry thermal models and silicon measurements before production tapeout. **Thermal simulation results are approximations** — reduced-order models, boundary condition assumptions, and material property variations introduce uncertainty. Thermal-aware floorplanning decisions should be verified with multiple simulation tools and, where possible, silicon validation.
- Self-hosted open-source solutions require proper PDK setup, tool chain integration, and domain expertise in thermal physics and chip design.

---

**Made for chip designers, thermal engineers, EDA researchers, and developers building open-source silicon design platforms.**  
Let's make microchip thermal layout architecture more open, accessible, and cool-running.
