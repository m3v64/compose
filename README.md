# Welcome!

welcome to my github repo, here i save and update my docker compose setup accross my multiple servers, i hope you find what you need.

![animation](./ayaya.gif)

## compose

A small collection of Docker Compose setups used to run services across two hosts: a main PC and several Raspberry Pi devices.

This repository keeps per-host Compose files organized under `pc/` and `rpi/` so you can quickly find and run the stacks you need.

## Layout

- `pc/` — Compose files and env for the main PC (subfolders: `gaming`, `management`, `media`, ...)
- `rpi/` — Compose files for Raspberry Pi hosts (subfolders: `dashboard`, `management`, `music`, `network`, ...)

## Quick start

1. Open the folder for the host you want `pc/` or `rpi/`.
2. Inspect the `docker-compose.yml` in the chosen subfolder.
3. Run:

```powershell
docker compose -f path\to\your\docker-compose.yml up -d
```

Replace `path\to\your\docker-compose.yml` with the file you selected.

## Notes

- This repository intentionally keeps multiple compose setups in a single place for convenience.
- Adjust `.env` files where present before starting a stack.

License: see `LICENSE`.
