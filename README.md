# homeassistant-euc

Homeassistant custom component for Electric Unicycles integration

## Supported wheels

Integration works with wheels supported by python euc library - KingSong only

## Prerequisites

Working bluez bluetooth stack (over DBUS). You can verify if it works by manual installation of python libraries and running:
```
pip install git+https://github.com/moleus/euc-kingsong-lib.git@main
python -m euc.cli
```
Above command should connect to nearby wheel and start displaying data.

## Instalation

1. Clone repo into custom_components folder
    ```sh
    cd custom_components
    git clone https://github.com/moleus/homeassistant-euc.git euc
    ```

2. In homeassistant go to Configuration / Integrations page and search for "Electric Unicycle" integration. After adding integration new sensors of basic wheel parameters should be visible.

Integration is read-only (only sensors are available)
