# GMS / MODFLOW Modeling Assistant — Gen II

**A source-grounded AI skill for practical groundwater modeling with Aquaveo GMS and MODFLOW.**

Created by **Kunyang Wang** · Version **1.0.0** · License **MIT** (original skill code/instructions only)

> **Independent project.** Not affiliated with, endorsed by, or supported by Aquaveo or the U.S. Geological Survey (USGS). GMS and MODFLOW names are used descriptively; their respective owners retain rights in their software, documentation, and marks.

## What this skill does

This skill helps students, groundwater modelers, and researchers make the next practical decision in a **GMS graphical workflow**, while distinguishing GMS interface instructions from the underlying MODFLOW engine.

- Build and check a conceptual groundwater model, lithologic structure, parameter zones, and computational grid.
- Configure boundaries and stresses (e.g., wells, rivers, recharge), stress periods, and time steps.
- Work with MODFLOW-2005, MODFLOW-NWT, and MODFLOW-USG **with engine-specific guidance**.
- Interpret groundwater parameters, solvers, model results, budgets, and convergence diagnostics.
- Plan calibration, validation, sensitivity tests, and practical troubleshooting.
- Reference official GMS and USGS documentation **when access is available**; clearly label advice that extends beyond verified manuals.

### Documentation scope / supported versions

The **default GMS interface baseline is 10.8** because that version was specified in the original skill. If your GMS version differs, tell the assistant the exact version/build so that it can check whether a menu path or model feature differs.

The version of **GMS** and the version of **MODFLOW** are separate questions: a technique described for one engine or version must not be assumed valid in another.

## Installation

### Use as a plugin

Clone or download this repository. Install the plugin using the **plugin-loading workflow supported by your host environment**, selecting the directory that contains the root `plugin.json`. Plugin host installation steps differ by product.

### Use as an Agent Skill

For a host that supports standard Agent Skills, install the directory:

`skills/gms-modflow-modeling/`

That folder includes the `SKILL.md` entry point and `lookup/` reference links. Installing the skill does not automatically enable web access.

## Examples

In Chinese:

> 我使用 GMS 10.8 和 MODFLOW-NWT。现在已经有钻孔资料与地层分区，如何设置网格、UPW 参数与补给边界？请给出下一步操作、检查要点，以及实际核对的手册链接。

In English:

> My MODFLOW-2005 groundwater model does not converge in transient simulation. What should I inspect in GMS first? Please separate verified manual instructions from modeling heuristics.

For a precise answer, include your **GMS version**, **MODFLOW engine**, **model purpose**, and, if possible, a screenshot of the relevant dialog, input settings, and/or simulation log.

## Documentation, sourcing, and availability

**No Aquaveo manual PDFs or other third-party copyrighted documents are bundled in this repository.** The skill relies on official websites when the host has browsing permissions. It contains **no prebuilt vector database or embedded search engine**.

- [GMS User Manual 10.8 — XMS Wiki](https://www.xmswiki.com/wiki/GMS:GMS_User_Manual_10.8) — primary reference for GMS 10.8 UI instructions.
- [GMS releases — Aquaveo](https://aquaveo.com/downloads-gms) — check available versions.
- [USGS MODFLOW and related programs](https://www.usgs.gov/mission-areas/water-resources/science/modflow-and-related-programs) — authoritative engine family information.
- [USGS MODFLOW-2005](https://www.usgs.gov/software/modflow-2005-usgs-three-dimensional-finite-difference-ground-water-model)
- [USGS MODFLOW-NWT](https://www.usgs.gov/software/modflow-nwt-a-newton-formulation-modflow-2005)

The online source inventory is also stored in `skills/gms-modflow-modeling/lookup/online-sources.json`.

**Important:** If the assistant has no web tool, it cannot verify exact GMS 10.8 menu paths against the online manual. In such cases, the skill instructs it to disclose that limitation and avoid inventing citations; users may supply screenshots or excerpts for a grounded answer.

## Licensing and attribution

All original skill instructions, JSON/YAML manifests, and original project-authored materials in this repository are licensed under the [MIT License](LICENSE).

The **GMS software, online user manuals, and USGS-linked resources are external**, are not redistributed here, and are not covered by the MIT license granted for this repository. The project does not grant a GMS software license. Please consult the original rights holders for third-party permissions and software licenses.

## Limitations

This is an **AI-assisted guidance tool**, not an engineering validation or software execution service. Advice must be reviewed against actual site measurements, hydrogeology, numerical assumptions, physical units, input/output files, and verified model behavior. Model calibration, mass balance, and convergence should be checked before results are used for research or decisions.

## Maintainer

**Kunyang Wang**  
GMS/MODFLOW Modeling Assistant Gen II
