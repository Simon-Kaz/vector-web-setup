# Attribution and fork lineage

This repository is a fork maintained for the VectorKit project
(https://github.com/Simon-Kaz/VectorKit) to self-host the Anki Vector web
setup / firmware flashing flow with no third-party dependency.

It is MIT-licensed (see `LICENSE`). The lineage:

- **Origin:** `digital-dream-labs/vector-web-setup` (MIT, (c) 2019-2020 Digital
  Dream Labs) -- the open-source Web-Bluetooth tool that configures Vector
  without the proprietary phone app. The valuable Web-Bluetooth GATT/RTS
  protocol code (`site/js/rts.js`) originates here and is unchanged.
- **Intermediate fork:** `bliteknight/vector-web-setup` -- added the firmware
  selection dropdown, OTA progress/error UI, and step-by-step instructions, and
  pointed the OTA backend at `ota.techshop82.com`. (That fork had removed the
  upstream `LICENSE` file; this fork restores it, since the upstream code
  remains MIT.)
- **This fork:** VectorKit. Repoints the setup app and OTA host at our own
  infrastructure and revamps the onboarding UX. See the VectorKit repo's
  `docs/web-setup.md` and the P5-01 task in `docs/PLAN.md`.

The MIT copyright notice for Digital Dream Labs is retained in `LICENSE` as
required; the VectorKit copyright line covers this fork's own changes.
