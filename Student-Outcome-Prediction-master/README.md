## Installation

There are several ways to install `uv`. The standalone installer is recommended.

### Standalone Installers

**macOS and Linux:**
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

**Windows (PowerShell):**
```bash
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

### Other Methods

You can also install `uv` with `pip`:
```bash
pip install uv
```

For more options like Homebrew, see the [official documentation](https://github.com/astral-sh/uv/blob/main/docs/getting-started/installation.md).

---

## How to Use (with uv)

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Ensure you have [uv](https://github.com/astral-sh/uv) installed**

   See the [Installation](#installation) section for details.

3. **Create and activate a virtual environment using uv**
   ```bash
   uv venv
   source .venv/bin/activate
   ```

4. **Install dependencies from lockfile**
   To install directly from the lockfile (recommended):
   ```bash
   uv pip sync
   ```

5. **Run your code**
   - For Jupyter notebooks:
     ```bash
     uv pip install ipykernel  # if not already installed
     ```
   - For Python scripts:
     ```bash
     python your_script.py
     ```

**Note:**  
- The project requires Python 3.12 (see `.python-version`).
- All dependencies are managed via `uv.lock`.