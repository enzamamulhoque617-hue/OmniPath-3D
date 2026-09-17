# OmniPath 3D 🔬✨
> **The Universal Interactive 3D Virtual Pathology & Molecular Diagnostic Lab Engine**

**OmniPath 3D** is an open-source, hands-on virtual laboratory platform engineered for medical laboratory science (MLS) students, diagnosticians, and educators to master manual clinical diagnostic procedures. Built directly for the browser using Three.js / WebGL and powered by Google Gemini, OmniPath 3D bridges manual procedural simulation with real-time AI supervision, protocol compliance, and biosafety hazard detection.

---

## 👨‍🔬 Creator & Institutional Credits

* **Lead Creator & Developer:** **Enzamamul Hoque**
* **Institution:** Mangaldai College
* **Department:** Department of Medical Laboratory and Molecular Diagnostic Technology (ML&MDT)

---

## 🌟 Key Features

* **Browser-Based 3D Bench:** Photorealistic, interactive glassware, instruments, and equipment rendered via Three.js with raycasting click-to-inspect controls.
* **Gemini AI Supervisor:** Real-time feedback engine that evaluates manual procedural steps, verifies reagent volumes, and tracks procedural timing.
* **Active Biosafety & Caution Engine:** Warns users instantly of procedural hazards (such as handling flammable solvents near open flames, omitting microcentrifuge balancing, or skipping cold-rack enzyme storage).
* **Multi-Department Scope:** Architected to support clinical protocols across the entire scope of pathology:
  * 🧫 **Microbiology:** Smear fixation, differential staining (Gram, Ziehl-Neelsen), and streak plating.
  * 🧬 **Molecular Diagnostics:** Pipetting workflows, cold-rack PCR Master Mix preparation, and sample loading.
  * 🔬 **Histopathology & Cytology:** Deparaffinization, hydration, and H&E staining series.
  * 🧪 **Clinical Biochemistry:** Colorimetric tests, spectrophotometric assays, and urinalysis.
  * 🩸 **Hematology & Blood Banking:** Manual cell counting via hemocytometer, peripheral blood smears, and ABO/Rh typing.

---

## 📁 Repository Structure

```text
OmniPath-3D/
├── protocols/                 # Ground-truth clinical protocols (JSON)
│   ├── microbiology/          # E.g., gram_stain.json
│   └── molecular/             # E.g., pcr_mastermix.json
├── backend/                   # Gemini AI Supervisor Server
│   ├── app.py                 # FastAPI service & evaluation pipeline
│   └── requirements.txt       # Python dependencies
├── frontend/                  # WebGL/Three.js interactive 3D client
│   └── index.html             # Virtual lab bench, 3D viewport & control UI
├── .gitignore                 # Excludes local environments and secrets
├── .env.example               # Template for API key configuration
└── README.md                  # Project documentation & setup instructions
