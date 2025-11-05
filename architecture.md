# Architektur & Pipeline

Pipeline: Load → Analyse (BPM) → Time-Stretch (Ziel/Original) → Equal-Power-Crossfade → Limiter → Export (WAV)

Module:
- dsp/bpm.py – BPM-Erkennung, Beat-Grid
- dsp/stretch.py – Zwei-Pass Time-Stretch (RubberBand → Librosa Fallback)
- dsp/xfade.py – Equal-Power-Crossfade, Filter-FX (Bass-Carve, Sweeps), Limiter
- app/ui.py – Streamlit-Frontend (Upload, Parameter, Mix-Start)

Methodik:
- GitHub Flow (Branches/PRs), PEP8 (flake8), Pytest (Unit/E2E), Pair Programming
