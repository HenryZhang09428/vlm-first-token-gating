A small pipeline for extracting first-token logits from a VLM (Qwen2.5-VL), training linear probes (safety / hallucination), and running a gated decoder with NORMAL / CAUTIOUS / REFUSE modes.

## Files
- main.py: entry point
- model_core.py: model loading + chat/generate helpers
- data_loader.py: dataset prep + memmap dataset
- probe.py: linear probe training/eval
- gating.py: gating policy + generation
- configs.py / utils.py: configs + utilities

## Quickstart
pip install -r requirements.txt
python main.py --help
