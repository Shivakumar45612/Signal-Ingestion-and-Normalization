# Brainwave-Ingestion

Minimal reference pipeline for real-time EEG/IMU signal ingestion, validation & normalization.

## Quick start

```bash
# 1) create project
bash create_folder.sh
cd brainwave_ingestion

# 2) bootstrap venv
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# 3) run mock generator
python src/mock_eeg_stream.py        # terminal ①

# 4) run adapter
python src/ingestion_adapter.py      # terminal ②

# 5) run normalizer
python src/signal_normalizer.py      # terminal ③
