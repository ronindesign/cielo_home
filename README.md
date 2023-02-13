# Cielo Home devices integration for HomeAssistant

[![hacs_badge](https://img.shields.io/badge/HACS-Default-41BDF5.svg?style=for-the-badge)](https://github.com/hacs/integration)
[![cielo_home](https://img.shields.io/github/release/bodyscape/cielo_home/all.svg?style=for-the-badge)](https://github.com/bodyscape/cielo_home/releases)
![Maintenance](https://img.shields.io/maintenance/yes/2023.svg?style=for-the-badge)
[![](https://img.shields.io/badge/MAINTAINER-bodyscape-red?style=for-the-badge)](https://github.com/bodyscape)

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?hosted_button_id=BKQL5JUGZBZXU)
[![Buy me a coffee](https://img.shields.io/static/v1.svg?label=Buy%20me%20a%20coffee&message=🥨&color=black&logo=buy%20me%20a%20coffee&logoColor=white&labelColor=6f4e37)](https://www.buymeacoffee.com/bodyscape)

A HomeAssistant custom integration to control Cielo Home devices.

## Functionality

![image](https://user-images.githubusercontent.com/30115568/217594793-e3009fee-bd3d-47aa-8638-dfc5af8b4e92.png)

A exemple of thermostat card i use : https://github.com/nervetattoo/simple-thermostat

![image](https://user-images.githubusercontent.com/30115568/218138232-3249b15e-ce08-4eee-bbeb-178d7e150caa.png)

``` yaml
# YAML
- type: custom:simple-thermostat
        entity: climate.basement
        step_size: 1
        layout:
          step: row
          mode:
            names: true
            headings: false
        header: true
        control:
          hvac:
            _name: Mode
          fan:
            _name: Fan Mode
          swing:
            _name: Swing Mode
          preset:
            _name: Preset Mode
```

# Installation

## With HACS

Click on the button below to automatically navigate to the repository within HACS:

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=bodyscape&repository=cielo_home&category=integration)

Alternatively, follow the steps below:

1. Click on the `Explore & Download Repositories` button and search for Cielo.
2. On the Cielo page, click on the `Download` button.

## Manual
Copy the `cielo_home` directory, from `custom_components` in this repository,
and place it inside your Home Assistant Core installation's `custom_components` directory.

`Note`: If installing manually, in order to be alerted about new releases, you will need to subscribe to releases from this repository. 

## Setup

Click on the button below to add the integration:

[![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=cielo_home)

Alternatively, follow the steps below:

1. Install this integration.
2. Navigate to the Home Assistant Integrations page (Settings --> Devices & Services)
3. Click the `+ ADD INTEGRATION` button in the lower right-hand corner
4. Search for `Cielo`
