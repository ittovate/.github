# ⏬ Installation
1. Install [Python](https://www.python.org/downloads/).
2. Install pre-commit: `pip install pre-commit`

# 🚀 Usage
1. Copy [starter file](https://github.com/ittovate/.github/blob/main/config/.pre-commit.yaml) to `config` directory in project root.
2. Install hooks: `pre-commit install --config ./config/.pre-commit.yaml`
3. Test hooks without committing: `pre-commit run --config ./config/.pre-commit.yaml --all-files`
4. Now, installed hooks should run each time you try to commit.

# ✅ Starter Hooks
- **pre-commit hooks:**
	- trailing-whitespace.
	- end-of-file-fixer.
	- check-yaml.
- **Local hooks:**
	- maven-checkstyle.
	- maven-test.
