# jenkins-practice

Sandbox for learning Jenkins pipelines.

## Layout
- `Jenkinsfile` — declarative pipeline (checkout → install → test → publish JUnit results)
- `tests/` — sample pytest suite the pipeline runs
- `requirements.txt` — Python test dependencies

## Run tests locally
```bash
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
pytest --junitxml=reports/junit.xml
```
