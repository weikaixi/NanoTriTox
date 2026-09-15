# NanoTriTox

Frozen NanoTriTox model and post-fit numerical analyses for three-endpoint nanomaterial toxicity prediction.

Download and extract **NanoTriTox-model-and-analysis.zip** in this repository. The archive includes the complete frozen model, inference engine, Python post-fit analyses, fixed reference predictions, example/template inputs, numerical tests, and the full README with main-figure correspondence.

The model is ready to use, with saved endpoint weights and MCP calibration pools applied directly during inference.

After extraction, install Node.js 22 or later and run from the extracted directory:

```sh
node tests/smoke.mjs
node src/run.mjs predict examples/prediction_example.csv predictions.csv
node src/run.mjs optimize CeO2 optimization.json
```

The full README explains Python requirements, MCP evaluation, SHAP, dose/time analyses, and the distinction between the final deployed model and saved domain-held-out predictions. The archive contains no credentials, manuscript documents, or original source publications.

Model and code are provided for research. Lower predicted toxicity is not a safety guarantee. Source-data terms remain applicable; no new software/data license has been assigned.

Public platform: https://nanotritox.cpmlab.cn
