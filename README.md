# Cooperative Perception and Fleet Operations for Level-4 Robotaxis in Mixed Southeast Asian Traffic

**Author:** Chee Woh (Terry) Chaw, Kuala Lumpur, Malaysia
**Prepared for:** PhD consideration, UCLA Mobility Lab (Prof. Jiaqi Ma)

## Summary

This repository outlines a proposed PhD research agenda on automated driving and new mobility. It focuses on how cooperative perception, mobility digital twins and electrified fleet operations can make Level-4 robotaxi services safe and scalable in dense, mixed traffic (motorcycles, pedestrians, informal road use) as found in Southeast Asia.

## Why this fits the UCLA Mobility Lab

The lab's published directions include cooperative perception, mobility digital twins, multimodal sensing, simulation, and the impacts of new mobility at scale. This proposal extends those themes to an under-studied setting: motorcycle-dense urban traffic, where single-vehicle sensing is limited by occlusion and unpredictable road users.

## Research questions

1. **Cooperative perception under occlusion.** How much does infrastructure-and-vehicle sensor sharing improve detection of vulnerable road users (motorcycles, pedestrians) in dense traffic, compared with ego-only perception?
2. **Mobility digital twin for pre-deployment validation.** Can a calibrated digital twin of a target city corridor predict L4 disengagement and near-miss rates before real-world deployment?
3. **Retrofit pathway.** What minimum sensor, compute and safety-monitor stack allows a production EV to be retrofitted for supervised L4 operation, and how should it be validated?
4. **Electrified fleet operations.** How do charging, vehicle-to-grid (V2G) participation and dispatch interact in a robotaxi fleet, and what is the effect on cost and grid load?

## Planned approach

| Phase | Work | Output |
|---|---|---|
| 1 | Literature review; reproduce an open cooperative-perception baseline on public datasets | Baseline results, reading notes |
| 2 | Build a small simulation of a mixed-traffic corridor with motorcycle-heavy agents | Open-source simulation scenarios |
| 3 | Evaluate cooperative vs ego-only perception in simulation | Comparison study |
| 4 | Prototype telemetry and data logging on real hardware | Data pipeline, field data |
| 5 | Fleet charging and V2G dispatch model | Model and analysis |

## Repository layout (planned)

```
docs/        proposal, reading list, notes
sim/         mixed-traffic simulation scenarios
perception/  cooperative-perception baselines
telemetry/   vehicle data logging prototype
fleet/       charging / V2G dispatch model
```

## Relevant background

- BE (Electrical & Electronic), University of Auckland.
- Former airline pilot (about 7,600 flying hours), with a safety-critical systems and human-factors perspective.
- Solar project supervision and business development (SFS Energy), focused on renewable energy and electrification.
- Ongoing work: EV vehicle-to-grid charger design, an automotive telemetry hardware prototype, and robotaxi research and development ("MyRobotaxi").

## Status

This is an early-stage proposal. No published results are claimed; the phases above are the intended plan. Code and data will be added as each phase is completed.

## Contact

Chee Woh (Terry) Chaw.email
 flytnc@gmail.com 
Whatsapp 60189521391
