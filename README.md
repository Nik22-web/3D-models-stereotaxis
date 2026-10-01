# 3D-models-stereotaxis

<img width="2090" height="1320" alt="Рисунок1" src="https://github.com/user-attachments/assets/04669b4d-bcec-47db-97a6-c9c8ada64770" />

# A 3D-Printed Open-Source Stereotaxic Platform for Orthotopic Glioma Cell Implantation into the Mouse Striatum

This repository contains the design files and assembly documentation associated with the manuscript:

**A 3D-Printed Open-Source Stereotaxic Platform for Orthotopic Glioma Cell Implantation into the Mouse Striatum**

**Authors:**  
Kurtova A.I., Esetov N.S., Khamitova Ya.D., Nosov M., Shipunova V.O.

---

## Overview

This repository provides the 3D-printable design files and assembly information required to reproduce and adapt the custom-built stereotaxic platform described in the associated manuscript.

The system consists of:

- one caliper-based needle manipulator;
- two mouse fixation frames;
- 3D-printed structural components;
- commercially available mechanical hardware.

The platform was developed for orthotopic implantation of glioma cells into the mouse striatum and was designed as a low-cost, modular alternative to conventional stereotaxic equipment.

---

## Repository version

The version of this repository corresponding to the manuscript and Supplementary Table S1 is tagged as:

`v1.0-manuscript`

This version should be used when reproducing the configuration described in the manuscript.

---

## Repository contents

The repository contains STL files for the following components developed for the present stereotaxic system:

### Mouse fixation frame support legs

- `first base platform leg.stl`
- `second base platform leg.stl`

### Caliper holder assembly

- `caliper holder.stl`
- `first depth gauge lock.stl`
- `second depth gauge lock.stl`

### Needle retainer

- `needle retainer base.stl`
- `clamping insert.stl`

### Tooth bar assembly

- `bite plate.stl`
- `manual adjustment knob.stl`
- `nose holder.stl`

Additional components of the mouse fixation frame are derived from an upstream open-source stereotaxic/anesthesia platform, as described below.

---

# Assembly Instructions

## 1. Needle retainer assembly

The needle retainer provides rigid fixation of the injection needle while allowing rapid insertion and replacement.

### Components

- needle retainer base;
- clamping insert;
- M3 screw;
- M3 hex nut;
- injection needle.

### Assembly

1. Insert the **M3 hex nut** into the recessed pocket of the clamping insert.
2. Position the **clamping insert** inside the lower slot of the needle retainer base.
3. Mount the assembled needle retainer onto the microscope holder.
4. Insert the **M3 screw** and thread it into the M3 hex nut.
5. Leave sufficient clearance for insertion of the injection needle.
6. Insert the needle and tighten the M3 screw until the needle is securely fixed.

Avoid excessive tightening to prevent damage to the printed components.

---

## 2. Mouse tooth bar assembly

The tooth bar assembly consists of:

- bite plate;
- nose holder;
- manual adjustment knob;
- M6 locking bolt;
- M6 receiving nut;
- retraction spring.

The bite plate contains a central aperture for positioning the upper incisors, while the nose holder prevents upward movement of the anterior part of the head.

### Assembly

1. Insert the **M6 receiving nut** into the recessed pocket of the bite plate.
2. Position the **retraction spring** inside the lower portion of the nose holder.
3. Insert the **nose holder** into the bite plate.
4. Mount the **manual adjustment knob** onto the M6 locking bolt.
5. Insert the locking bolt through the upper opening of the bite plate.
6. Thread the bolt into the M6 receiving nut.
7. Rotate the manual adjustment knob to adjust the position of the nose holder and the clamping force.

---

## 3. Mechanical caliper installation

The mechanical vernier caliper is used to determine vertical needle displacement.

### Installation

1. Attach the **caliper holder** to the upper rail of the microscope stand.
2. Insert the upper jaw of the mechanical caliper into the holder.
3. Verify that the caliper depth gauge moves freely through the corresponding slot in the microscope stand rail.
4. Adjust the caliper position if necessary.
5. Remove the original screw securing the movable microscope stage.
6. Install the **depth gauge retainer** in its place.
7. Insert the caliper depth gauge into the retainer.
8. Secure the depth gauge using the clamping plate.
9. Fasten the assembly using the original microscope-stage screw.
10. After correct alignment has been confirmed, secure the caliper mounting components with adhesive to prevent displacement during stereotaxic procedures.

---

## 4. Needle and catheter installation

Before use:

1. Insert a 29- or 30-gauge needle into polyethylene or PTFE catheter tubing with an inner diameter of approximately 0.3 mm.
2. Place the catheter–needle assembly vertically into the needle retainer.
3. Secure the needle using the locking screw.
4. Connect the opposite end of the catheter tubing to a precision syringe pump.
5. Fill the fluid pathway with PBS and verify that no air bubbles remain before injection.

---

# Fabrication and configuration options

Several components can be produced either by 3D printing or by machining.

## Ear bars

Two alternatives are described:

### Printable version

- fabrication method: mSLA / DLP / SLA;
- material: photopolymer resin;
- STL file: `3DStereotax_earbar.stl`.

### Experimentally used version

- fabricated by machining;
- starting material: steel rod, Ø5 mm × 200 mm.

---

## Support legs

Two printable support-leg designs are provided:

- `first base platform leg.stl`
- `second base platform leg.stl`

These components can be fabricated by FDM using PETG or another suitable FDM polymer.

In the experimentally used configuration, the corresponding support legs were machined from steel.

The starting material for each type of metal support leg was:

**Metal block, 40 × 40 × 100 mm**

---

# Experimental and fully printable configurations

Two configurations should be clearly distinguished.

## Experimentally used configuration

The configuration used in the experiments described in the manuscript consisted of:

- two mouse fixation frames;
- one needle manipulator;
- metal ear bars;
- metal support legs.

As of July 29, 2026, the total material cost of this configuration was:

**USD 63.44**

## Fully printable configuration

A lower-cost configuration can be assembled using the provided and referenced STL files with:

- two mouse fixation frames;
- one needle manipulator;
- photopolymer ear bars;
- FDM-printed support legs.

As of July 29, 2026, the estimated total material cost of this configuration was:

**USD 40.07**

The fully printable configuration is an alternative to the exact configuration used in the reported experiments and should be identified as such when reproduced or described.

---

# Upstream design acknowledgement

Selected components of the mouse fixation frame were adapted from the open-source **Anesthesia Surgery System** developed by the Optogenetics and Neural Engineering (ONE) Core at the University of Colorado School of Medicine.

The upstream project is available at:

https://optogeneticsandneuralengineeringcore.gitlab.io/ONECoreSite/projects/AnestesiaSurgerySystem/

The ONE Core project itself is a remix of earlier open-source rodent stereotaxic designs. The project page identifies a 3D-printed rodent stereotaxic device developed by Lex Kravitz as one upstream source, which itself was based on the Mouse Head Holder designed by John Everett Martin.

For the present stereotaxic system, only selected components of the mouse fixation frame were adapted from this upstream project.

The following elements were developed for the present work:

- needle manipulator;
- tooth bar assembly;
- caliper holder assembly;
- needle retainer;
- support-leg designs;
- overall integration of the stereotaxic system.

The manuscript-associated upstream STL files are:

- `StereotaxONECoreBasev3.stl`
- `StereotaxONECoreSliderv3.stl`
- `3DStereotax_earbar.stl`

The upstream files referenced in Supplementary Table S1 correspond to commit:

`7993f017aa33881c48f564a40fe3eec5df085773`

Third-party and upstream materials remain subject to their original authorship, licensing, and reuse conditions.

The reuse permissions described below for the original materials in this repository do not replace or override the terms applicable to upstream materials.

Users should consult the original upstream project for any additional reuse conditions.

---

## ONE Core acknowledgement

The ONE Core project page requests acknowledgement of the facility in publications using its work.

In the context of the present work, we acknowledge the Optogenetics and Neural Engineering (ONE) Core at the University of Colorado School of Medicine for providing the original open-source design basis for selected components of the mouse fixation frame.

The ONE Core is part of the NeuroTechnology Center at the University of Colorado School of Medicine. According to the original project page, the facility is funded in part by the School of Medicine and by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154.

---

# Use and reuse

The original design materials created by the authors and provided in this repository may be freely:

- downloaded;
- copied;
- used;
- reproduced;
- modified;
- adapted;
- redistributed;
- shared;
- incorporated into other designs;
- used for research;
- used for educational purposes;
- used for commercial or non-commercial purposes.

Users are free to modify the authors' original files and create derivative designs.

The requested condition for reuse is appropriate attribution.

If these files, modified versions of them, or designs substantially derived from them are used in a publication, presentation, thesis, report, repository, or other scholarly output, please cite the associated article.

These reuse terms apply only to original materials for which the authors of this repository have the right to grant such permissions.

Upstream and third-party materials remain subject to their own terms.

---

# Citation

If you use the original design files provided in this repository or substantially derived designs, please cite:

**Kurtova A.I., Esetov N.S., Khamitova Ya.D., Nosov M., Shipunova V.O.  
A 3D-Printed Open-Source Stereotaxic Platform for Orthotopic Glioma Cell Implantation into the Mouse Striatum.  
Journal of Neuroscience Methods.**

Final bibliographic information and DOI will be added after publication.

---

# Modifications and derivative designs

Users are encouraged to modify and improve the system according to their experimental requirements.

Modified versions should be clearly identified as derivative designs.

Changes in:

- geometry;
- dimensions;
- materials;
- manufacturing method;
- component arrangement;
- assembly procedure

may affect the mechanical or experimental performance of the system.

Modified versions should therefore not be described as experimentally validated by the original authors unless they correspond to the configuration evaluated in the associated publication.

---

# Disclaimer

The design files and documentation are provided without warranty of any kind.

Users are responsible for:

- verifying the mechanical integrity of reproduced or modified components;
- determining whether the system is suitable for their intended application;
- complying with applicable institutional and ethical requirements;
- complying with animal-use regulations;
- following appropriate laboratory and surgical safety procedures.

---

# Contact

For questions regarding the design or associated manuscript:

**Anastasia I. Kurtova**  
Corresponding author

