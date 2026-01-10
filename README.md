# ECG Diagnosis Partner

A comprehensive web application for systematic ECG interpretation, designed as a clinical co-pilot for cardiologists.

![ECG Diagnosis Partner](https://img.shields.io/badge/ECG-Diagnosis%20Partner-dc2626?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-222?style=flat-square)

## Features

### 🔬 Systematic ECG Analysis
- Step-by-step framework: Rate → Rhythm → Axis → Intervals → P wave → QRS → ST → T wave
- Quick-select buttons for common findings
- Automatic differential diagnosis generation based on documented findings

### 📊 Clinical Calculators
- **QTc Calculator** - Bazett, Fridericia, and Framingham formulas
- **Quick Axis Determination** - Lead I/aVF polarity method
- **Sgarbossa Criteria** - STEMI diagnosis in LBBB (with Smith-modified criteria)
- **CHA₂DS₂-VASc Score** - Stroke risk in atrial fibrillation
- **HAS-BLED Score** - Bleeding risk on anticoagulation

### 📖 Diagnostic Criteria Reference
- STEMI (with coronary territory mapping)
- NSTEMI/Unstable Angina
- Atrial Fibrillation & Flutter
- WPW / Pre-excitation
- Bundle Branch Blocks (LBBB, RBBB)
- LVH & RVH criteria
- Brugada Pattern
- Long QT Syndrome
- Hyperkalemia & Hypokalemia
- Pulmonary Embolism
- Pericarditis
- Digoxin Effect/Toxicity

### 💊 QT-Prolonging Drugs Database
Comprehensive reference organized by drug class:
- Antiarrhythmics
- Antibiotics
- Antipsychotics
- Antidepressants
- Antiemetics
- Opioids

### 🤖 AI-Powered ECG Analysis
- Upload 12-lead ECG images for AI-assisted interpretation
- Uses Claude (Anthropic) for pattern recognition
- Systematic analysis with differential diagnoses
- Requires your own API key (stored locally)

### 📋 Report Generation
- One-click copy of structured interpretation report
- Includes all documented findings and differentials

## Quick Start

### Option 1: Use Online (GitHub Pages)
Visit: `https://[your-username].github.io/ecg-diagnosis-partner`

### Option 2: Run Locally
1. Download `index.html`
2. Open in any modern browser
3. No server or installation required

## Deployment to GitHub Pages

1. Create a new repository on GitHub
2. Upload `index.html` to the repository root
3. Go to Settings → Pages
4. Set Source to "Deploy from a branch"
5. Select `main` branch and `/ (root)` folder
6. Click Save
7. Your app will be live at `https://[username].github.io/[repo-name]`

## Usage Guide

### Basic Workflow
1. Enter **Clinical Context** (age, sex, presenting complaint)
2. Input **ECG Parameters** (intervals, rate)
3. Use **Systematic Analysis** to document findings
4. Review generated **Differentials**
5. **Copy Report** for documentation

### For LBBB with Chest Pain
1. Go to Analysis → Sgarbossa tab
2. Check applicable criteria
3. For Smith-modified, enter ST elevation and S wave depth
4. Score ≥3 or positive Smith ratio suggests STEMI

### For Atrial Fibrillation
1. Document AFib in systematic analysis
2. Go to Calculators tab
3. Calculate CHA₂DS₂-VASc for stroke risk
4. Calculate HAS-BLED for bleeding risk
5. Review anticoagulation recommendations

### AI Analysis
1. Go to AI Analysis tab
2. Enter your Anthropic API key
3. Upload ECG image (high-quality 12-lead recommended)
4. Click "Analyze with AI"
5. Review systematic interpretation

## Technical Details

- **Framework**: React 18 (via CDN)
- **Styling**: Custom CSS with dark theme
- **Fonts**: IBM Plex Sans & IBM Plex Mono
- **Dependencies**: None (single HTML file)
- **Storage**: Local only (no server required)
- **AI**: Anthropic Claude API (optional)

## Clinical Disclaimer

⚠️ **This tool is for clinical decision support only.**

- Always correlate with clinical presentation
- Expert review and clinical judgment required
- AI interpretations require verification
- Not a substitute for formal cardiology training
- Not FDA approved for diagnostic use

## Contributing

Contributions welcome! Areas for improvement:
- Additional diagnostic criteria
- More risk calculators
- Improved differential logic
- Mobile responsiveness
- Additional QTc formulas

## License

MIT License - See LICENSE file for details.

## Acknowledgments

- ECG criteria based on current ACC/AHA/ESC guidelines
- QT drug database informed by CredibleMeds.org
- Sgarbossa criteria and Smith modification from original publications

---

Built with ❤️ for cardiologists, by cardiologists.
