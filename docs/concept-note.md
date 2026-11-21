# Safe Streets Addis: A Privacy-First Road Safety System for Addis Ababa

Road safety as preventive medicine. An open, citizen proposal for Addis Ababa and other African cities: a citizen contribution for a better tomorrow.

Author: Dr. Temesgen Endalew Legesse, MD, MSc HPE, PMP. Affiliation: Africa Digital Health Academy (ADHA), Tibon Hub. The views are the author's.
Version 0.3, DRAFT FOR DISCUSSION, 20 November 2026
Licence: Creative Commons Attribution 4.0 (CC BY 4.0). Anyone may use and adapt this proposal, with credit to the author.
Contact for implementation or collaboration: info@drtemesgen.com

**Who is proposing this, and why.** The author is an Ethiopian physician, digital-health strategist and certified project manager, Board Chairman of the Africa Digital Health Academy (ADHA), an Ethiopian civil society organisation that trains health and digital-health professionals across Africa. ADHA, through its innovation hub Tibon Hub, supported the work. Road traffic injury is one of the leading preventable causes of death of young Ethiopians, so this proposal treats road safety as preventive medicine: the cheapest trauma care is the crash that never happens.

The proposal is offered as a free contribution. The author holds no interest in any equipment supplier and would take no share of fine revenue. He is willing to advise without payment during preparation; any later role would be for the implementing institutions to decide under their own rules.

---

## 1. Summary

About 400 people die on Addis Ababa's roads every year by police count, and police data are known to under-count. Pedestrians are 86 percent of those killed. City officials report that speeding contributed to nearly half of fatal crashes in 2023/24, and roadside surveys from December 2020 to September 2024 found 44 percent of vehicles above the enforced limit [1][2].

Addis already has most of the parts of a modern enforcement system:
- new national number plates with an RFID chip and a QR code, issued since 11 June 2026 for new vehicles [3];
- a traffic management centre built to control 130 intersections with hundreds of cameras [4];
- telebirr payment of traffic penalties since 2022, and a national point-based penalty system since 2025 [5][6];
- a digital fine system that already notifies drivers and owners by SMS (since January 2025) [27];
- Council of Ministers Regulation 557/2024, which already sets an urban maximum of 50 km/h and lets the competent authority sign lower limits (Articles 25(4) and 25(7)), with penalty points and licence suspension, and allows electronic enforcement and a national points database (Articles 95(12) and 95(13)) [7].

The next step is to join them. Safe Streets Addis proposes:

1. For every vehicle: cameras at paired roadside sites read the number plates of all cars, minibuses, buses, trucks, motorcycles and government vehicles to measure average speed, and detect red-light and lane offences. Where the new plates carry a readable chip, the chip is a second check against cloned or dirty plates.
2. Existing city cameras gain automated detection of likely offences. A trained human controller confirms each one before any notice is issued.
3. Public minibus taxis and fleets report their speed and any tampering. Following distance and lane keeping are measured for driver coaching first, not fines.
4. Only drivers with a confirmed offence are identified; every other vehicle's records are deleted within hours. The owner or driver is looked up only after an offence is confirmed, and can pay through any approved channel, including telebirr, or appeal.
5. The same coded traffic data helps the city roads authorities predict congestion and warn drivers about road closures in advance.

**Impact.** Once the system covers the city, about 40 deaths and about 190 serious injuries would be avoided each year in the central case. The range is wide: 8 to 97 deaths. These are modelled estimates (Section 7).

**Cost and money.** The system can start small. A lean, warning-only pilot on one corridor, using existing cameras and drivers' own phones, needs an estimated USD 27,000 to 125,000 in cash, on top of staff time, existing cameras and hosting given in kind by the City, the Institute and partners. Import duty is not included. A full city-wide system with new roadside sites and sealed taxi units costs an estimated USD 8 to 44 million, and its fines would cover only about 40 to 60 percent of its annual cost. A lean version, built on cameras the city already owns, costs far less. Whether its fines would exceed its cost is not yet known; the pilot will measure it. If there is a surplus, the proposal is that it goes to a city Road Safety Fund (Section 8).

**The invitation.** Public bodies, partners and researchers who wish to test, adapt or implement this design, starting with a lean pilot of 6 to 9 months (Section 10), are welcome to contact the author.

## 2. The problem

| Indicator | Value | Source |
|---|---|---|
| Ethiopia road deaths, WHO estimate vs police record (2021) | 21,258 vs 3,971 | [8] |
| Cost of road crashes to Ethiopia | about USD 5.1 billion, about 5 percent of GDP | [9] |
| Addis police-recorded deaths | 463 (2015/16) to 401 (2023/24) | [1][10] |
| Pedestrians among Addis deaths | 86 percent; 78 percent of pedestrians killed are male; 45 percent of all those killed are aged 20 to 39 | [1][2] |
| Vehicles above the enforced limit, Addis | 44 percent (roadside surveys, Dec 2020 to Sep 2024) | [2] |
| Fatal crashes where speeding contributed, Addis | nearly half (2023/24, as reported) | [1] |

WHO finds that speed contributes to around one third of road deaths in high-income countries and up to one half in low- and middle-income countries. Nine in ten pedestrians survive being hit at 30 km/h; fewer than half survive at 45 km/h [11][12].

What earlier measures taught: in the 2020-21 limiter programme, more than 30,000 speed limiters were fitted nationally, but only 46 percent were in proper use [13]. A device that caps speed cannot be checked without data. A system that reports tampering and links it to a consequence can.

## 3. What other countries teach

| Country | What was done | Result | Lesson for Addis |
|---|---|---|---|
| Rwanda | Nationwide speed cameras from April 2021; fines payable by web or USSD | Associated with a 38 percent fall in monthly road deaths | Cameras work in a low-income African setting [14] |
| Norway and other countries | Average-speed control between two points | Killed-or-seriously-injured crashes down about 49 to 56 percent at treated sites (few studies) | Two plate readings are enough [15][28] |
| Kenya | Speed governors on minibuses (2003); instant camera fines (2026) | Governors: no measurable effect. 2026 fines: launched in the week of 9 March, paused by court order on 12 March | Tamper alerts, legal basis, human review and notice must come first [16][17] |
| Uganda | Digital plates and trackers, contractor paid from plate fees and fines | About USD 257 million investment; plate price raised about five-fold; slow delivery | Government owns data and design; never pay a contractor from fines [18] |
| United States (New York) | AI bus-lane cameras with human review | About 3,800 wrong tickets in a warning period, all refunded | Test in warning mode; audit the reviewers [19] |

## 4. How it works

**Roadside.** Paired camera sites on main corridors measure average speed. Junction cameras detect red-light running. The first sites go where pedestrians die: school zones, markets and main crossings.

**Speed limits set centrally.** The central system holds the legal limit for each place where a detector or camera stands, and applies it to that location. The city can set lower limits for school zones, hospitals and markets, change limits by time of day, and add temporary limits for roadworks or events from the control room, without touching the roadside equipment. The same limits are sent to the taxi app, so drivers are warned before they speed.

**Existing cameras.** A small computer added to each existing camera turns video into coded movement data: position in lane, speed and gap to the vehicle ahead. Only that data travels to the centre in normal running, so new sites do not need fast links; the routine data is small enough for the 2G network. Evidence clips need 3G, 4G or fibre. A central model flags likely offences. Only then is the short video clip and the plate reading retrieved, and a human controller decides.

**Taxis and fleets.** In the pilot, a phone app on volunteer drivers' own phones records speed and harsh braking, and gives feedback. Later, licensed public transport may carry a sealed unit that also reports tampering, with the cost subsidised or leased.

**Following distance.** A safe gap grows with speed; a fixed rule of 3 to 5 metres is not safe above walking pace (about half a second at 30 km/h). The pilot measures the gap in seconds and uses it for coaching. Whether it becomes an offence, at what threshold and above what speed, is for Government to decide after the pilot.

**Human control room.** Trained controllers review every flagged event, work to written criteria with a limit on cases per hour, and log each decision. A second reviewer checks disputed cases. Error rates are published.

**Everything is documented.** Every flag, controller decision, speed-limit change, identity request, notice, payment, appeal and refund is recorded in a signed audit trail, so that any later change can be detected. Each record shows who did what and when. Auditors, courts and the data regulator can check it, and the summary is published each year.

**From offence to fine.**

| Step | Rule |
|---|---|
| First months | Warning notices only |
| Who is liable | The registered owner, unless the owner names the driver. Points go only to a driver who is named and does not contest, or is identified by evidence. This builds on Articles 93 and 95(3) of Regulation 557/2024 but needs a clear rule |
| Notice | SMS and official app, with a paper notice if unread after 14 days. Never a payment link in a message |
| Payment | Any approved channel: telebirr, banks, other licensed mobile money. Regulation 557/2024 now requires payment within 10 working days, with interest after that; because camera notices arrive by message, the proposal suggests a longer period for camera cases |
| Appeal | Regulation 557/2024 provides a complaint to the traffic office within 2 working days, then to the appropriate body within 5 working days; a person who has paid may complain to the Ministry, whose decision is final at the administrative level (Art. 95(5) and 95(7)). The proposal adds an independent review officer and access to the competent court, with payment paused during appeal |
| Evidence | Only certified and regularly calibrated devices |
| Equal treatment | All vehicles, including government vehicles; any exemption listed in law |
| Repeat offences | Penalty points, then retraining, then suspension under existing rules |

## 5. Privacy and public trust

All vehicle data is treated as personal data under the Personal Data Protection Proclamation 1321/2024 [20]. The system is built so that the city learns how traffic moves without knowing who is moving, unless a confirmed offence requires it.

- **Coded identifiers.** Vehicles appear only under coded identifiers that change over time. Records of law-abiding vehicles are deleted automatically within hours.
- **Identity held separately.** The link from code to person is held by a separate body and used only for a confirmed offence, with a logged decision.
- **One purpose.** The data is used for road safety and traffic management only. Any other use needs a separate law.
- **Road-facing cameras.** Roadside cameras capture plates and vehicles only. In-vehicle cameras face the road, and footage stays in the unit.
- **Written into the rules.** European courts accepted average-speed control only where a specific law set these limits. A court in Lower Saxony, Germany, stopped the first system in 2019 until the state passed such a law. Austria's Constitutional Court struck down a law that allowed much wider use of the data [21][22]. Ethiopia should put the deletion rule and the purpose limit in the regulation itself.

## 6. Traffic flow and planning

Can safe following distance reduce traffic jams? In part. Experiments show stop-and-go waves can start from drivers' own braking, and smoother following can dampen them. One field test reported up to 15 percent higher flow, but with one automated vehicle among about 20 cars on a closed ring road [23]. The pilot will measure the effect for human drivers in Addis, not assume it.

The coded movement data gives the City Roads Authority, the Transport Bureau and the Transport Management Centre a live picture of travel times and incidents on main corridors. They can predict congestion, time roadworks, clear incidents faster, and warn drivers of planned closures days ahead by SMS, USSD and navigation apps.

## 7. Expected impact

| Once city-wide | Low | Central | High |
|---|---|---|---|
| Fall in average speed | 2 percent | 5 percent | 8 percent |
| Deaths avoided per year | 8 | 40 | 97 |
| Serious injuries avoided per year | 56 | 194 | 372 |
| Value of deaths and injuries avoided per year | USD 1.4 m | USD 5.8 m | USD 12.4 m |

Injury numbers use the 2020/21 count of 2,847 serious injuries [10]. The model links a fall in average speed to fewer deaths using the established power model [24]. It was built on rural roads and fits city streets less well, so the low case uses a smaller effect. The share of deaths the system can reach (50, 70 and 85 percent) is the author's assumption. Value uses the iRAP rule (70 times GDP per capita for a death, a quarter of that for a serious injury) [25]. The pilot is too small to prove a change in deaths; it will measure speed and injury crashes.

Enforcement is one part of a Safe System (safe roads, safe speeds, safe vehicles, safe road users). It complements, and does not replace, the pedestrian crossings, footways and speed-calming works in the City's road safety strategy.

## 8. Cost, money and the proposed Road Safety Fund

Indicative estimates at 160 birr per US dollar, to be replaced by quotes:

| Item | Low | Central | High |
|---|---|---|---|
| Lean pilot, cash only (one corridor, existing cameras, phone app, warning-only) | USD 27,000 | | USD 125,000 |
| Full pilot (24 sites, 2,000 sealed taxi units) | USD 2.0 m | USD 3.1 m | USD 4.8 m |
| Full city-wide capital cost | USD 8.4 m | USD 19.3 m | USD 44.0 m |
| Full city-wide annual cost (capital over 7 years plus running) | USD 2.9 m | USD 6.3 m | USD 14.0 m |
| Fine revenue in year 3 | USD 1.1 m | USD 3.7 m | USD 7.5 m |
| Fines as share of annual cost (full system) | 39 percent | 58 percent | 54 percent |

Low cost goes with low revenue, and high with high.

What this means:
- The full hardware system does not pay for itself. It must be budgeted as a public safety service, with capital from Government and partners.
- On reported deaths and injuries, the value of harm avoided (Section 7) is a little below the annual cost of the full system in the central case (USD 5.8 million against 6.3 million) and well below it in the low case. This is the second reason to start with the lean version: it seeks a similar fall in speed from cameras the city already owns, at a much lower cost. The pilot will measure the fall in speed on one corridor. Police counts are known to miss deaths, so the true benefit is likely higher.
- **The lean path may leave a surplus, and the pilot will test this.** Built on cameras the city already owns, on the new plates and on phones, it costs a fraction of the full system. The pilot itself is warning-only and earns nothing. If later fine revenue exceeds cost, the proposal is that the surplus goes to a city **Road Safety Fund**. Where fine revenue goes is for the City and the Ministry of Finance to decide.
- The fund would pay for what saves pedestrians: crossings, footways, lighting and school zones. Its income should fall as driving improves, so it should pay for one-time works, not salaries or other lasting costs. It publishes a public report each year.
- To keep trust, no operator, controller or supplier may earn more by issuing more fines. Running costs come from a fixed budget line. Fines go to the account designated by the City and the Ministry of Finance.
- Fine revenue should fall as driving improves. That is success, not failure.

## 9. Who does what

| Institution | Proposed role |
|---|---|
| Addis Ababa City Transport Bureau (traffic management sector) | Proposed lead agency and operator, to be confirmed [26] |
| Addis Ababa Transport Management Centre / the City's traffic control centre | Hosts the control room |
| Addis Ababa City Roads Authority | Roads, signs, closures; main user of planning data; pedestrian works from the proposed Road Safety Fund |
| Ethiopian Artificial Intelligence Institute | Builds and tests the AI models with Ethiopian engineers; owns the national capability |
| Addis Ababa Police Commission | Legal enforcement and roadside follow-up |
| Driver and Vehicle Licensing and Control Authority | Registry, licences, suspension |
| Ministry of Transport and Logistics | National policy, plates, point-based record |
| Ministry of Finance | Any external financing; destination of fine revenue |
| Ethiopian Communications Authority | Data protection oversight |
| Information Network Security Administration | Cyber security standards and security audit of the system |
| National Bank of Ethiopia | Oversight of payment channels |
| Ethiopian Metrology Institute (to be confirmed) | Certification and calibration of devices |
| Africa Digital Health Academy (Tibon Hub) | Could advise without payment in preparation, and train controllers and driver coaches if the institutions wish |
| Licensed telecom and payment operators | Connectivity and payment, selected under procurement rules |
| Taxi associations | Co-design, driver coaching, consent for the phone pilot |
| Universities | Independent evaluation |

## 10. The proposed path

| Phase | Time | What happens | Decision gate |
|---|---|---|---|
| 0. Agree | 1-3 months | Lead agency named; legal review of camera evidence, owner liability and data protection; taxi association consultation | Lead agency and legal path agreed |
| 1. Lean pilot | 6-9 months | One corridor; existing cameras with AI units; one average-speed pair; phone app with 200 volunteer taxis; warning-only for the whole pilot | Speed and injury crashes vs a comparison corridor; error and appeal rates; public opinion |
| 2. City pilot | 12-18 months | Three corridors; more sites; first sealed units for licensed public transport | Published evaluation |
| 3. City-wide | 2-3 years | All main corridors; Road Safety Fund operating, if approved | City decision |

**Next step:** any city or national body interested in a lean pilot can contact the author at info@drtemesgen.com.

## 11. Main risks

| Risk | Response |
|---|---|
| No clear legal basis yet for camera fines and owner liability | Phase 0 legal review; warning-only until the rule is in place |
| Wrong fines from AI errors | Human confirmation, warning-only start, published error rates, easy appeal and refund |
| Old plates without chips | Cameras read all plates; the chip is only a second check |
| Fear of surveillance | Coded data, deletion, single purpose, separate identity body, published audits |
| Cost to taxi owners | Phone app first; subsidised or leased units later; coaching before fines |
| Fake fine messages | No payment links; reference lookup through official channels only |
| Incentive to over-fine | No earnings linked to fine volume; fixed operating budget |
| Roles are still settling after the 2026 restructuring | One lead agency confirmed in writing |

## References (accessed or searched 20 November 2026)

1. Addis Fortune. Road Injuries Increase by 35pc, with Pedestrians Most Affected. 13 April 2025. https://addisfortune.news/road-injuries-increase-by-35pc-with-pedestrians-most-affected
2. Johns Hopkins IIRU / Bloomberg Initiative for Global Road Safety. Status Summary 2024: Road Safety Risk Factors, Addis Ababa. https://publichealth.jhu.edu/sites/default/files/2025-02/ENGLISH_ADDIS_ABABA_SSR-1.pdf
3. The Reporter Ethiopia. Ethiopia Begins Issuing New National Vehicle Plates. 11 June 2026. https://www.thereporterethiopia.com/51124/
4. Addis Fortune. Capital builds smart traffic management center. 7 January 2023. https://addisfortune.news/capital-builds-smart-traffic-management-center
5. Developing Telecoms. Ethiopia's telebirr now supports penalty payment for drivers. 7 March 2022. https://developingtelecoms.com/telecom-technology/telecom-devices-platforms/13065-ethiopia-s-telebirr-now-supports-penalty-payment-for-drivers.html
6. Shega. Ethiopia integrates fuel, fares and fines in sweeping digital reform. 14 May 2025. https://shega.co/news/ethiopia-integrates-fuel-fares-and-fines-in-sweeping-digital-reform
7. Road Transport Traffic Control Council of Ministers Regulation No. 557/2024. Federal Negarit Gazette, 30th Year No. 57, 19 August 2024. https://justice.gov.et/en/law/road-transport-traffic-control-council-of-ministers-regulation/
8. WHO. Global status report on road safety 2023: Ethiopia country profile. https://cdn.who.int/media/docs/default-source/country-profiles/road-safety/road-safety-2023-eth.pdf
9. iRAP. Ethiopia Takes Major Step Toward Safer Roads with RSIFS, ERA and iRAP Partnership. 19 June 2026. https://irap.org/ethiopia-takes-major-step-toward-safer-roads-with-rsifs-era-and-irap-partnership/
10. Johns Hopkins IIRU / BIGRS. Status Summary 2022, Addis Ababa. https://publichealth.jhu.edu/sites/default/files/2025-03/2022_ADDIS-SSR.pdf
11. WHO. Managing speed. 2017. https://www.who.int/publications-detail/managing-speed
12. Johns Hopkins IIRU / BIGRS. Risky Road Behaviors in Addis Ababa. January 2019. https://www.vitalstrategies.org/wp-content/uploads/2019/05/Addis-R7-GAR-Final-English_Pages.pdf
13. The Reporter Ethiopia. Less than 2000 vehicles fitted with speed limiters in Addis. 9 October 2021. https://www.thereporterethiopia.com/12087/
14. Delavary M, et al. Assessing the effect of automated speed enforcement and comprehensive measures on road safety in Rwanda. Traffic Injury Prevention 25(7):947-955, 2024.
15. Hoye A. Speed cameras, section control, and kangaroo jumps: a meta-analysis. Accident Analysis and Prevention 73:200-208, 2014. https://www.saferresearch.com/node/1299
16. Habyarimana J, Jack W. State vs Consumer Regulation: An Evaluation of Two Road Safety Interventions in Kenya. NBER Working Paper 18378, 2012. https://www.nber.org/system/files/working_papers/w18378/w18378.pdf
17. The Star (Kenya). High Court halts NTSA's Instant Fines system pending review. 12 March 2026. https://www.the-star.co.ke/news/2026-03-12-court-halts-ntsas-instant-fines-system
18. The Independent (Uganda). Fresh details on digital number plates. 21 April 2024. https://www.independent.co.ug/fresh-details-on-digital-number-plates/
19. NBC New York. MTA's A.I. bus cameras issue thousands of mistaken parking violations. 26 November 2024. https://nbcnewyork.com/investigations/mta-bus-camera-issue-mistake-parking-violations/6020986/
20. 5A Law Firm via Legal500. Ethiopian Personal Data Protection Law (Proclamation 1321/2024). https://www.legal500.com/intelligence/ethiopia/privacy/ethiopian-personal-data-protection-law-proclamation-1321-2024-business-compliance-guide
21. Dr. Datenschutz. Section Control: Geschwindigkeitskontrolle auf dem Pruefstand (Lower Saxony rulings 2019). https://www.dr-datenschutz.de/section-control-geschwindigkeitskontrolle-auf-dem-pruefstand/
22. Austrian Constitutional Court. G 72-74/2019. https://www.vfgh.gv.at/downloads/Bulletin_2019-3_AUT-2019-3-003_G_72-74_2019__ua.pdf
23. Stern RE, et al. Dissipation of stop-and-go waves via control of autonomous vehicles: Field experiments. Transportation Research Part C 89, 2018. https://arxiv.org/abs/1705.01693
24. Cameron MH, Elvik R. Nilsson's Power Model connecting speed and road trauma. Accident Analysis and Prevention 42(6):1908-1915, 2010. https://pubmed.ncbi.nlm.nih.gov/20728642/
25. iRAP Toolkit. Crash Costing. https://toolkit.irap.org/management/crash-costing/
26. Capital Ethiopia. Addis Ababa reassigns traffic management duties across three agencies. 22 October 2026. https://capitalethiopia.com/2026/10/22/addis-ababa-reassigns-traffic-management-duties-across-three-agencies/
27. Addis Fortune. Traffic Management Overhaul Digitises Fines, Parking Fees. 5 January 2025. https://addisfortune.news/traffic-management-overhaul-digitises-fines-parking-fees
28. Hoye A. Safety effects of section control: an empirical Bayes evaluation. Accident Analysis and Prevention 74:169-178, 2015.

Method and assumptions are in the Technical Annex and the cost model, which come with this note. A list of sources is available on request.
