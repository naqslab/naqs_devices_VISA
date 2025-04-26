# VISA

## Directory structure

```text

└── VISA/
    ├── .gitignore
    ├── pyproject.toml
    ├── README.md
    ├── LICENSE.txt
    ├── CITATION.cff
    ├── naqs_devices/ # note: must be same as in the parent naqs_devices repo to be in the same namespace
    │   └── VISA/
    │       ├── __init__.py
    │       ├── register_classes.py
    │       ├── labscript_devices.py
    │       ├── blacs_tabs.py
    │       ├── blacs_workers.py
    │       └── runviewer_parsers.py
    └── docs/
        └── index.rst

```

## Usage

This module leverages pvisa to communicate to VISA compatible devices and is meant to be inherited by a labscript device's components. The module also provides GUI widgets for an instrument's status bytes, as well as the option for analog and digital outputs.
