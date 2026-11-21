# Safe Streets Addis - Technical Annex

Version 0.3, 20 November 2026. Author: Dr. Temesgen Endalew Legesse (Africa Digital Health Academy, Tibon Hub). Licence CC BY 4.0.
Companion to the concept note. Shared under an open licence so that the design stays free for public use. The licence covers these documents only and grants no rights in third-party technology. Figures marked "estimate" are planning assumptions.

## A1. Design principles

1. Build on what Addis already owns: cameras, the traffic management centre, new plates, telebirr penalty payment, the point-based record.
2. Send data, not video. The routine data is small enough for the 2G network. Evidence clips for flagged cases need 3G, 4G or fibre.
3. Coded by default; identity only after a human-confirmed offence.
4. Open, technology-neutral specifications; open-source software where possible; Ethiopian engineers own the models.
5. Warning-only first. No fine until legal basis, accuracy and appeal route are proven.
6. Every vehicle is treated the same. Roadside sites read every plate: private cars, minibuses, buses, trucks, motorcycles and government vehicles. Taxis and fleets get one extra layer (speed and tamper reporting); they are not the only target.

## A2. Components

| Component | What it does | Off-the-shelf? | Difficulty |
|---|---|---|---|
| Average-speed pair | Two plate-reading cameras at a known distance; GPS-synchronised clocks; speed = distance / time | Yes, mature worldwide | Low to medium |
| Red-light and lane cameras | Plate reading plus signal-phase or lane-line detection | Yes | Low to medium |
| RFID plate reader (optional) | Reads the chip in new plates as a second check against cloned or dirty plates | Yes, but the Ethiopian plate chip type is unknown | Medium (needs Ministry specification) |
| AI unit on existing cameras | Small computer (for example a Raspberry Pi with an AI accelerator, about USD 160-400 with enclosure and power) runs open-source detection and tracking; outputs coded tracks only | Parts yes; the integration is new work | Medium to high: the core job for the AI Institute |
| Central speed-limit register | One table in the central system: each detector or camera location with its legal limit, special zones (school, hospital, market), time-of-day rules and temporary limits (roadworks, events). Every speed check uses the limit for that place and time; changes are logged; limits are pushed to taxi apps and units | Yes (standard database and map tools) | Low |
| Central flagging model | Reads coded tracks from many cameras; flags weaving, tailgating, line crossing, red-light running, speeding | No; built and trained locally | High |
| Evidence retrieval | For a flagged event only, pulls a 10-20 second clip and the plate reading over 3G/4G or fibre | Yes (standard video systems) | Low |
| Control room | Screens, case queue, written criteria, decision log, second review, audit sampling | Yes (case-management software) | Low; staffing and training are the real work |
| Identity service | Separate body holds the code-to-plate key; resolves only confirmed cases; logged | Simple software; the institution is the work | Medium (governance) |
| Notice and payment | SMS + official app + paper fallback; payment through telebirr, banks, licensed mobile money by reference number | Yes; telebirr penalty payment exists since 2022 | Low to medium |
| Taxi phone app (pilot) | Phone GPS and motion sensor: speed, harsh braking; weekly feedback to the driver. The association sees only group results unless the driver agrees to share his own | Yes (many open-source examples) | Low |
| Sealed taxi unit (later) | GPS, motion sensor, forward camera, tamper alert; 4G with 2G fallback | Yes (dashcam-ADAS class, about USD 250-500) | Medium |
| Planning dashboard | Corridor travel times, incident alerts, closure notices to drivers | Yes (open-source tools; Waze for Cities for closures) | Low to medium |

Overall: about 70 percent of the system is standard technology already used in other countries. The new and hardest parts are the AI layer on existing cameras, the central flagging model, and joining the institutions (registry, payment, legal basis). The institutional work is harder than the technical work.

## A3. Data flow

1. Camera or unit sees a vehicle. The edge unit records a coded track: random identifier valid for minutes, lane position, speed, gap to the vehicle ahead, time. About 30 bytes per vehicle, sent when the vehicle leaves the view.
2. The central model reads tracks from many cameras and flags a possible offence.
3. The system requests the short clip and plate reading for that event only.
4. A controller confirms or rejects, using written criteria. A second reviewer checks a random sample and all disputed cases.
5. For a confirmed case only, the identity service links the code to the plate and the registered owner.
6. Notice sent; owner pays, names the driver, or appeals.
7. Records of law-abiding vehicles are deleted within hours. Evidence is kept only for the appeal period. Aggregated, de-identified statistics are kept for planning.

## A4. Bandwidth (estimate)

- Edge camera: 30 bytes x 1,000 vehicles per hour = about 30 KB per hour. Fits 2G (GPRS) easily.
- Taxi unit or app: event records of 50-150 bytes; about 0.1-0.3 MB per day.
- Video clips: only for flagged events, over 3G/4G or fibre.
- Hardware should be 4G with 2G fallback so it survives network upgrades.

## A5. Following distance

| Speed | 1-second gap | 2-second gap | Stopping distance (1 s reaction, 5 m/s2 braking) |
|---|---|---|---|
| 30 km/h | 8 m | 17 m | about 15 m |
| 50 km/h | 14 m | 28 m | about 33 m |
| 80 km/h | 22 m | 44 m | about 72 m |

Pilot rule: coaching feedback when the gap is under 2 seconds above 30 km/h. Following distance stays a coaching signal until Government decides, after the pilot, whether it becomes an offence.

## A6. Accuracy and audit

- Every model is tested on Addis footage before use: day, night, rain, faded markings, minibuses, bajaj, animals, pedestrians.
- Publish each quarter: flags raised, share confirmed by humans, appeals, appeals upheld, refunds.
- Controllers: cap on cases per hour; rotation; random re-review of 5 percent of decisions; integrity checks.
- Independent audit once a year by a university or the Ethiopian Communications Authority.

## A6b. Audit trail

Every event is written to an append-only, digitally signed log: flags raised, controller decisions and reasons, second reviews, speed-limit changes (who, when, why), identity requests and their legal basis, notices, payments, appeals, refunds, model versions and accuracy tests. Logs are kept for the period set in regulation, are available to auditors, courts and the Ethiopian Communications Authority, and feed the annual public report. Personal data inside the log follows the same deletion rules as the rest of the system.

## A7. Security

- Data hosted in Ethiopia. Encryption in transit and at rest. Evidence records signed so that any later change can be detected.
- The identity key is held in a locked security device (hardware security module) by the separate identity body.
- Security testing by outside experts before go-live; incident report to the regulator within 72 hours as the data law requires.

## A8. Lean pilot bill of materials (estimate)

| Item | Low USD | High USD |
|---|---|---|
| Plate-reading cameras for one average-speed pair (4 units, existing poles) | 4,000 | 10,000 |
| AI units on 10-20 existing corridor cameras | 2,000 | 8,000 |
| Installation, power, mounting, SIM and data | 2,000 | 8,000 |
| Baseline speed survey, two corridors | 2,000 | 6,000 |
| Legal opinion and data protection assessment (Phase 0) | 0 (in kind) | 10,000 |
| Taxi phone app for 200 volunteer taxis | 0 (built with the AI Institute or a university) | 15,000 |
| Server and software (open source, in-country) | 3,000 | 10,000 |
| Controllers and coaching (seconded city staff) | 0 (in kind) | 10,000 |
| Independent evaluation and public communication | 10,000 | 30,000 |
| Contingency (15 percent, rounded up) | 4,000 | 18,000 |
| Total cash (staff, cameras, poles and hosting in kind; import duty not included) | 27,000 | 125,000 |

## A9. Open questions to answer in Phase 0

1. Legal basis. Regulation 557/2024 (Gazette 19 Aug 2024) allows electronic enforcement and a national points database (Art. 95(12)-(13)), sets 10 working days to pay and a Ministry decision on complaints (Art. 95). Still to settle: its fine schedule (Schedule B is missing from published copies), camera evidence rules, owner liability, and a longer payment period for camera notices. A reported 2025 regulation with a 40 km/h urban default could not be found in the Gazette.
2. The chip type and read specification of the new plates.
3. How many cameras the traffic management centre runs, and whether it accepts new data feeds.
4. Lead agency after the October 2026 restructuring.
5. Number of minibus taxis and their share of crashes (Police Commission data).
6. Payment and identity interfaces: telebirr biller terms, bank channels; whether Fayda is needed at all.
