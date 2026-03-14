# Unreal ML-Agents Trainers

The `ueagents` Python package is part of the Unreal ML-Agents Toolkit. `ueagents`
provides a set of reinforcement and imitation learning algorithms designed to be
used with Unreal Engine environments. The algorithms interface with the Python API
provided by the `ueagents_envs` package.

## Notice

This package is inspired by Unity's ML-Agents Toolkit. The primary differences are:
- `ueagents` has been updated to import from `ueagents_envs` instead of `mlagents_envs`.
- Changes were made to support Unreal Engine, with references to Unity replaced with Unreal.
- SideChannels are not supported yet, and the code has been adjusted accordingly.

All credit for the foundational work goes to Unity's ML-Agents Toolkit team.

## Installation

Install the `ueagents` package with `uv`:

```sh
uv venv --python 3.12
.venv\Scripts\activate
uv pip install pip setuptools wheel
uv pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu130
uv pip install ueagents
```

If you are developing from source, install `ueagents_envs` in editable mode first:

```sh
cd ../ue-agents-envs
uv pip install -e .

cd ../ue-agents
uv pip install -e .
```

## Usage & More Information

For more information on the Unreal ML-Agents Toolkit and how to instrument an Unreal
scene with the Unreal ML-Agents SDK, check out the main
[Unreal ML-Agents Toolkit documentation](https://unrealmlagents.readthedocs.io/en/latest/).

## Credit

[Unity ML Agents](https://github.com/Unity-Technologies/ml-agents)
