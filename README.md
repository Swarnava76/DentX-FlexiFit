# DentX FlexiFit V5

**Conceptual dental X-ray sensor housing and adjustable positioning system**

DentX FlexiFit is a mechanical CAD concept developed in FreeCAD. The design explores a compact sensor-shaped enclosure with a removable protective face cover and a detachable positioning accessory made from a sensor-side clip, positioning arm, aiming ring, and ring collar.

> **Project status: Concept / preliminary prototype.** This repository does not contain evidence of a functioning X-ray detector, validated detector electronics, clinical performance, regulatory approval, or manufacturing readiness. It is not intended for clinical use.

---

## Project overview

The project focuses on the mechanical packaging and positioning concept around an intraoral dental imaging sensor. The submitted FreeCAD V5 document contains:

- A six-component conceptual assembly.
- A separate preliminary housing-cavity feature.
- A dummy PCB representation and four PCB support-post solids.
- Conceptual electronics and detector-interface placeholders.
- A battery cassette, charging connector, detector readout/interface, cable strain-relief, and charging-port placeholders.
- An exploded concept assembly.
- A BOM and design-review spreadsheet.
- Two TechDraw pages: General Assembly and Housing/PCB Detail.

## Design concept

### 1. ComfortEdge
A rounded enclosure concept with a removable protective face cover. The cover and oral-contact interface require material, sealing, cleaning, biocompatibility, and durability validation.

### 2. FlexiPosition
A detachable positioning concept consisting of:
- Sensor-side clip
- Positioning arm
- Aiming ring
- Aiming ring collar

The assembly is intended to explore sensor positioning and handling. Its ergonomics, strength, adjustment range, and fit have not been validated.

### 3. SmartConnect
The CAD file includes conceptual placeholders for detector interface/readout, wireless communication, power management, battery packaging, and charging. These are packaging representations only; they do not demonstrate working electronics or wireless functionality.

---

## CAD component inventory

| Component / group | Description |
|---|---|
| Rounded sensor dummy housing | Main enclosure representation |
| Removable protective face cover | Separate protective-cover component |
| Detachable sensor-side clip | Interface to the positioning accessory |
| Positioning arm | Connects the clip and aiming assembly |
| Positioning aiming ring | Positioning accessory component |
| Aiming ring collar | Collar associated with the aiming ring |
| Preliminary cavity feature | Separate housing feature representing an internal cavity |
| Dummy PCB | Placeholder labelled **32 × 22 × 1.6 mm** |
| PCB support posts | Four separate support-post solids |
| Electronics placeholders | CMOS detector interface, wireless communication, power management, and battery envelope |
| Final concept refinement | Battery cassette, charging connector, detector interface/readout, cable strain-relief collar, and charging-port interface |
| Exploded concept assembly | Exploded representations of 20 components |
| BOM and Design Review | Spreadsheet object stored in the FreeCAD document |

The values above are CAD labels or conceptual placeholders, not verified production specifications.

## Preliminary design values

| Item | Value in the concept | Status |
|---|---:|---|
| Dummy PCB | 32 × 22 × 1.6 mm | Placeholder label; verify against the selected PCB |
| Battery cassette | 19 × 11 × 3.8 mm | Concept placeholder |
| Sensor body envelope | 41.9 × 30.4 × 4.5 mm | Preliminary concept baseline; requires verification |
| Housing corner radius | 5 mm | Preliminary concept baseline |
| PCB support posts | 4 solids | Present in CAD; dimensions and mounting fit require verification |

Do not use these values for fabrication until they have been checked against the selected detector, PCB, tolerances, clearances, and material/process requirements.

---

## Repository structure

A suggested repository layout is:

```text
DentX-FlexiFit/
├── README.md
├── CAD/
│   ├── DentX_FlexiFit_V5_Finalized.FCStd
│   └── DentX_V5_Drawing_Scale_Improvement.FCMacro
├── Documentation/
│   ├── DentX_FlexiFit_Technical_Design_Report_V5.docx
│   └── DentX_FlexiFit_Technical_Design_Report_V5.pdf
├── Drawings/
│   ├── General_Assembly.pdf
│   └── Housing_and_PCB_Detail.pdf
├── Images/
│   ├── assembly-isometric.png
│   ├── exploded-view.png
│   └── technical-drawings.png
└── LICENSE
```

Only add files that you have actually exported or created. The image and PDF filenames above are suggested names; replace them with your actual exported files. Do not add a license unless you have chosen one and have the right to apply it.

## Software and tools

- **FreeCAD 1.1.4** — 3D CAD modelling and TechDraw documentation.
- **FreeCAD TechDraw** — General assembly and housing/PCB detail sheets.

## Current documentation

The FreeCAD project includes:
- General Assembly drawing page with top, front, and isometric views.
- Housing and PCB Detail drawing page with housing top, front, isometric, and PCB/support-post top views.
- A BOM and design-review spreadsheet object.

Before release, review the drawing scale, sheet layout, dimension annotations, view labels, and title-block readability. Export the final sheets to PDF from FreeCAD and include those exported PDFs in `Drawings/`.

## Engineering limitations and safety

This is a **mechanical concept CAD project**, not a complete dental X-ray imaging device.

- The CAD placeholders do not establish a working CMOS detector, scintillator, detector readout chain, ADC, image-processing system, wireless link, or battery electronics.
- A general-purpose microcontroller is not a substitute for specialised X-ray detector and readout electronics.
- Housing dimensions, cavity geometry, wall thickness, PCB mounting, cover retention, and positioning interfaces require engineering verification.
- Materials intended for oral contact require appropriate biological evaluation and cleaning/disinfection assessment.
- Electrical safety, electromagnetic compatibility, software, risk management, and regulatory requirements need assessment by qualified specialists.
- Do not expose a homemade prototype to X-rays or use it on a person. Any future X-ray testing must be conducted only in an appropriately equipped facility under qualified radiation-safety and engineering supervision.

Potential standards to assess with a qualified compliance specialist include IEC 60601-1, IEC 60601-1-2, IEC 60601-2-65, ISO 10993-1, and IEC 62304. Applicability and current editions must be confirmed for the intended device and market.

## Future development

1. Select a real detector module and obtain its verified mechanical and electrical specifications.
2. Update the housing and cavity around the selected detector and PCB.
3. Dimension and tolerance the housing, cover, clip, arm, ring, collar, and support posts.
4. Verify assembly clearances, retention features, mechanical strength, and serviceability.
5. Complete a sourced BOM with materials, manufacturing processes, quantities, and part references.
6. Define the detector/readout, power, charging, and data interfaces with qualified electronics engineering input.
7. Improve and export dimensioned TechDraw drawings.
8. Conduct formal design, risk, and regulatory reviews before any physical detector testing.

## Project status

**Version:** V5  
**Stage:** Conceptual mechanical CAD and design documentation  
**CAD source:** FreeCAD `.FCStd` document  
**Validation:** Not clinically or experimentally validated

DentX_FlexiFit_V5_Finalized.FCStd

---

## Disclaimer

DentX FlexiFit is presented for educational, conceptual engineering, and portfolio demonstration purposes only. It is not a medical device, does not provide diagnostic imaging, and must not be used for patient care, clinical diagnosis, or unsupervised radiation testing.
