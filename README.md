# radar-sim

**radar-sim** is a Rust project focused on simulating how radar systems work.  
It aims to model radar signal generation, propagation, reflection, and detection — and then visualize these phenomena in real time using the [Bevy](https://bevyengine.org/) game engine.  

```scss
  ┌──────────────┐
  │              │
  │   RADAR TX   │
  │              │
  └──────┬───────┘
         │  (Transmit Pulse)
         ▼
   ~~~~~~~~►►►►►►►►►►   (Electromagnetic Wave)
         ▲
         │  (Echo / Return)
  ┌──────┴───────┐
  │              │
  │   RADAR RX   │
  │              │
  └──────────────┘
```

## Goals

- **Educational:** Understand radar fundamentals (pulse-Doppler, range resolution, clutter, noise).
- **Experimental:** Simulate different radar scenarios — static objects, moving targets, multiple radars.
- **Visual:** Use Bevy to display radar sweeps, detections, and target tracking in a 2D or 3D environment.
- **Interactive:** Eventually allow users to tweak parameters (frequency, PRF, antenna pattern) and observe effects.
- **Game Potential:** Build radar-based gameplay mechanics once the simulation is solid.

## Tech Stack

- **Rust** – For performance and safety in numerical simulation.
- **Bevy** – To visualize radar sweeps, targets, and tracking in real time.
- **(Future)** DSP libraries – For FFT-based signal processing and clutter rejection.
- **(Future)** ECS systems – To handle multiple radars, targets, and environments.

## Roadmap

- [ ] Build a basic simulation engine for radar pulses & returns.
- [ ] Simulate range, velocity, and signal strength for point targets.
- [ ] Add noise and clutter models.
- [ ] Implement signal processing (matched filter, Doppler FFT).
- [ ] Visualize detections in Bevy.
- [ ] Add interactive controls (frequency, PRF, scan rate).
- [ ] Experiment with turning it into a radar-themed game.

## Contributing

Contributions are welcome!
If you have experience in radar systems, DSP, Rust, or Bevy, feel free to open issues, share ideas, or submit PRs.

## License

MIT — do whatever you want, just give credit.
