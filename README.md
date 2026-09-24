<div align="center">

<h1>IPLp : IPL Match Predictor</h1>

<p>
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=flat-square">
  <img src="https://img.shields.io/badge/scikit--learn-ML-orange?style=flat-square">
  <img src="https://img.shields.io/github/license/Terminay/IPLp?style=flat-square">
  <img src="https://img.shields.io/github/last-commit/Terminay/IPLp?style=flat-square">
</p>

</div>

This is a learning project for ML. It has the ability to predict IPL winners by watching previous year data upto 2024, although many things have changed since then in cricket.

If you have any questions or would like to contact me: email on -> _tanayonduty at gmail dot com_


| Branch | Contents |
|--------|----------|
| `main` | ML package + CLI |
| `docs` | Static documentation (GitHub Pages) |
| `site` | Web UI + HTTP API |

```powershell
py -3.12 -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python -m ipl_predictor download-data --force
python -m ipl_predictor train pre
python -m ipl_predictor train matchday
```

Web (local): `pip install -r requirements-api.txt` then `uvicorn web.api.main:app --port 8000`
