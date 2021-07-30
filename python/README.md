## HOW TO CREATE PYTHON VIRTUAL ENVIRONMENT IN VSCODE WINDOW

1. Run in the current location:

```python -m venv .venv```

2. Select new interpreter python in the .venv/script folder path

3. Open new powershell to confirm the path (.venv) in the powershell

4. Start pip install

#### REFERENCES
https://code.visualstudio.com/docs/python/environments

https://stackoverflow.com/questions/54106071/how-can-i-set-up-a-virtual-environment-for-python-in-visual-studio-code

https://techinscribed.com/python-virtual-environment-in-vscode/

## CONDA FOR MAC M1 VSCODE
To install at current location

```conda create --prefix ./envs```

or with packages

```conda create --prefix ./envs scipy```

Required to restart Terminal to take effect

```conda init zsh```

Activate 

```conda activate ./envs```

