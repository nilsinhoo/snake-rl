# Notes zum Github

## Prerequisites

Für das Repo werden Numpy 1.x und PyTorch 1.x benötigt. Mit `pyenv` können mehrere Python-Versionen parallel verwaltet werden. `pyenv` sollte global installiert werden.

Installation von `pyenv`

```bash
brew update
brew install pyenv
```

Installation überprüfen

```bash
pyenv --version
```

Python 3.10 ist die höchste mit PyTorch 1.x kompatible Python-Version und kann über folgenden Befehl mit pyenv installiert werden.

```bash
pyenv install 3.10.11
```

Installierte Python-Versionen überprüfen:

```bash
pyenv versions
```

Nun sollte eine virtuelle Umgebung eingerichtet und aktiviert werden.

```bash
python3 -m venv venv
source venv/bin/activate
```

Innerhalb der virtuellen Umgebung wird mittels `pyenv` die Python-Version 3.10 aktiviert.

```bash
pyenv local 3.10
```

Nun kann die Installation der benötigten Python Bibliotheken erfolgen.

```bash
pyenv exec python3 -m pip install numpy==1.26.4 torch==1.13.1 pygame matplotlib ipython
```

Nach der Installation können die Python-Executables ausgeführt werden.

```bash
pyenv exec python3 snake_game_human.py
```
