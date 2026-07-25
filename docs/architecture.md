# Architecture

Atlas is organized around three product layers:

## Capture

Browser workers open pages, wait for stable layout and fonts, discover same-site routes and UI states, and save browser evidence.

## Reconstruction

The captured structure becomes a versioned design document containing editable frames, text, controls, images, SVGs, and safe Auto Layout groups.

## Verification

The reconstructed design is rendered and compared with the source browser capture. Mismatch regions are classified so the system can retry or retain a correction case.

## Planned operating model

The local plugin currently coordinates the final import and validation handoff. The long-term architecture moves orchestration to durable cloud jobs so Atlas can continue when Figma, the laptop, or the local network is unavailable. Figma then reconnects as a client that imports completed, verified work.

Private implementation details, service endpoints, schemas, and worker code are intentionally omitted from this repository.
