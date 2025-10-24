# hass-epaper-waveshare

## Introduction

This repository contains our configuration for **ESP-Home**, which we use with our Home Assistant system.

We have a **Waveshare** e-ink display connected to an **ESP32**.

We use it to display temperature and humidity values, as well as the time and upcoming calendar events.

![A Picture of Display](https://github.com/tobibot/hass-esp32-epaper/blob/dev/assets/v_2024-01-30.jpg?raw=true)

## Description

The version in the bottom right corner is essentially the date and time, to determine if an update was successful.

The drop changes its appearance depending on the amount of rain on the current day. Initially it is empty (`< 5 l/d`), then filled black (`< 15 l/d`), finally the flood picture appears (`>= 15 l/d`).

### Variables for positioning

I recently discovered that it is possible to use variables to position elements, thus making it easier to move things to other places on the screen. I will replae all hard coded numbers in the future.

## Resources

Helpful resources can be found on the [ESPHome website](https://esphome.io/components/display/#display-engine).

The Icons are all from [Material Design Icons](https://pictogrammers.com/library/mdi/). On my setup most of the icons work while I found some not working.

[A blogpost I took inspiration from](https://smarterkram.de/1407/)

[The hass.io forum thread about E-paper displays](https://community.home-assistant.io/t/e-paper-display/138625/55)