VENV_DIR = .venv
PYTHON = python3
PIP = $(VENV_DIR)/bin/pip
TARGET = myscript.py

all: $(VENV_DIR) $(TARGET)

$(VENV_DIR):
    $(PYTHON) -m venv $(VENV_DIR)
    $(PIP) install -r requirements.txt

$(TARGET): $(VENV_DIR)
    $(PYTHON) $(TARGET)

clean:
    rm -rf $(VENV_DIR) __pycache__
