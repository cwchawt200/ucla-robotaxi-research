# Research Proposal

**Title:** Cooperative Perception and Electrified Fleet Operations for Level-4 Robotaxis in Mixed, Motorcycle-Dense Urban Traffic

**Applicant:** Chee Woh (Terry) Chaw
**Target group:** UCLA Mobility Lab (Prof. Jiaqi Ma)
**Status:** Draft research agenda, not completed work

---

## 1. Motivation

Level-4 robotaxi services have grown mainly in cities with relatively structured traffic. Much of the world's urban mobility, including Southeast Asia, looks different: dense mixed traffic with many motorcycles, pedestrians crossing informally, frequent occlusion, and variable infrastructure quality. A vehicle that relies only on its own sensors is limited by line of sight in these scenes. Cooperative perception, where vehicles and roadside units share sensing information, is a promising way to extend what an automated vehicle can see. However, most public cooperative-perception benchmarks come from lower-density, car-dominated settings, so it is unclear how well current methods transfer to motorcycle-dense traffic.

Operating a robotaxi fleet also depends on electrification. Charging schedules, grid load and the possibility of vehicle-to-grid (V2G) participation affect cost and availability, and are rarely studied together with perception and safety.

## 2. Research questions

1. **Occlusion and vulnerable road users.** How much does cooperative perception improve detection and tracking of motorcycles and pedestrians compared with ego-only perception, and where does it fail?
2. **Transfer to dense mixed traffic.** How do existing cooperative-perception methods, trained on current datasets, degrade when evaluated on motorcycle-dense scenarios, and what changes (data, architecture, training) close the gap?
3. **Digital twin for pre-deployment validation.** Can a calibrated mobility digital twin of a target corridor predict near-miss and disengagement behaviour well enough to guide deployment decisions?
4. **Retrofit pathway.** What minimum sensing, compute and safety-monitoring stack supports supervised L4 operation on a retrofitted production EV, and how should it be validated?
5. **Fleet energy operations.** How do charging policy, dispatch and V2G participation trade off against service level and grid impact?

## 3. Proposed methodology

**Phase 1: Foundations (months 1-6).** Review the literature (see `READING_LIST.md`). Reproduce one or two open cooperative-perception baselines (for example V2X-ViT or Where2comm) on public datasets such as OPV2V and V2V4Real, to establish a working pipeline and reference numbers.

**Phase 2: Mixed-traffic scenarios (months 6-12).** Build a simulation of a motorcycle-dense urban corridor, using CARLA and/or SUMO or MetaDrive-style tools, with parameterised motorcycle behaviour (lane splitting, filtering, sudden crossing). Generate cooperative-perception data with and without roadside units.

**Phase 3: Evaluation and method development (months 12-24).** Quantify the benefit and failure modes of cooperative perception in these scenarios. Explore improvements such as occlusion-aware fusion, robustness to localisation error and communication delay, and training with synthetic-plus-real data.

**Phase 4: Digital twin and real data (months 18-30).** Build a digital twin of one real corridor. Compare simulated and real sensor data collected with a low-cost logging prototype, and assess how well the twin predicts risky interactions.

**Phase 5: Fleet energy model (months 24-36).** Model charging and V2G dispatch for a small robotaxi fleet and combine it with the service-level results above.

## 4. Expected contributions

- An open set of motorcycle-dense mixed-traffic scenarios for cooperative-perception research.
- A benchmark of existing cooperative-perception methods on those scenarios, with an analysis of failure modes.
- Methodological improvements for occlusion and vulnerable-road-user detection under realistic communication constraints.
- A digital-twin validation workflow and a low-cost data-logging setup.
- A fleet charging and V2G model linked to service quality.

## 5. Why I am a good fit

- BE in Electrical & Electronic Engineering (University of Auckland).
- About 13 years as an airline pilot (about 7,600 flying hours), giving direct experience with safety-critical systems, procedures and human factors.
- Current work in solar and renewable energy project supervision, and hands-on projects in EV vehicle-to-grid charger design and an automotive telemetry hardware prototype.
- Ongoing robotaxi research and development, including study of a retrofit path for a production EV.
- Based in Kuala Lumpur, a real example of the dense mixed traffic this research targets, with access to local road and operating context.

## 6. Risks and mitigations

| Risk | Mitigation |
|---|---|
| Limited real-world cooperative data in dense traffic | Start with simulation; use public datasets for baselines; collect small real datasets with a low-cost logger |
| Sim-to-real gap | Calibrate the digital twin against real logs; report the gap explicitly |
| Compute limits | Begin with lightweight baselines and shared lab resources |
| Scope too broad | Treat perception (Q1-Q2) as the core; Q3-Q5 are extensions prioritised with an advisor |

## 7. Note on scope

This document is a proposed direction, written to start a conversation. The research questions and timeline are meant to be refined with an advisor to match the group's priorities and funding.
