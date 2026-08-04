# 📖 Lesson Plan — Raspberry-Pi-Tinkering

> **Chain K — Hardware & Systems Foundations** | A Pi as a real computer: headless setup, SSH, GPIO, sensors, and small always-on services worth running at home.

## What This Project Is

Run a Pi as a real headless server and as a bridge to physical hardware via GPIO, hosting something you actually keep running.

## Learning Objectives

By the end I can:

1. Set up a Pi headless and connect over SSH with key auth.
2. Read sensors and control components through **GPIO**.
3. Run a service reliably on boot with systemd.
4. Understand SD card wear and mitigate it.
5. Keep a small always-on service healthy.
6. Recover a Pi that has become unreachable.

## Software You Will Use

- Raspberry Pi OS Lite.
- Python with gpiozero.
- systemd.
- SSH.

## Build Order

1. Flash the OS with SSH and wifi pre-configured; boot headless.
2. Harden SSH with key-based auth.
3. Wire a sensor and read it from Python.
4. Write a service and enable it at boot.
5. Deploy something genuinely useful (DNS blocker, monitor, dashboard).
6. Simulate a power cut and confirm it recovers cleanly.

## Common Mistakes to Avoid

- Leaving password SSH and default credentials enabled.
- Writing logs constantly to the SD card until it fails.
- Under-powered supplies causing silent corruption.
- Wiring GPIO at the wrong voltage.
- No plan for recovery when it stops responding.

## Check Your Understanding

The quiz covers headless setup, SSH hardening, GPIO safety, systemd services, and SD wear.

## Why This Matters (Industry Application)

The Pi teaches Linux administration and IoT fundamentals on hardware where mistakes are cheap. Edge
computing and embedded systems are growing fields, and the habits — headless administration, remote access,
service management — are exactly what server work requires.

## Reflection Questions

- What is genuinely worth running always-on at home, and what is just novelty?
- How does managing this Pi resemble managing a production server?
