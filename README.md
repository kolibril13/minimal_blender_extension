Hello


1. use quickstart from the VS Code Blender Extension


# Install Blender from https://www.blender.org/download/
# Install uv 
curl -LsSf https://astral.sh/uv/install.sh | sh
mkdir blender_python_workshop && cd blender_python_workshop
uv venv --python 3.11
uv pip install jupyterlab blender_notebook
uv run blender_notebook install --blender-exec="/Applications/Blender.app/Contents/MacOS/Blender"
uv run jupyter lab

uv run blender_notebook remove
uv run jupyter kernelspec list
