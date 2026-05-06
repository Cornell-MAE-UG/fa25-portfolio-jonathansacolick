---
layout: project
title: ODP Final Report - Team Dragonfly
subtitle: Scraping Away Spotted Lanternflies
description: Extendable scraper for spotted lanternfly egg masses
image: /assets/images/dragonfly/final_prototype_exhibit_photo.png
technologies: Fusion360
---

<style>
  table {
    border-collapse: collapse !important;
    border-spacing: 0 !important;
    width: 100% !important;
    margin: 0 0 1.4rem 0 !important;
    font-size: 0.92rem;
  }

  table th,
  table td {
    border: 1px solid #555 !important;
    padding: 7px 9px !important;
    vertical-align: top !important;
  }

  table th {
    font-weight: 700 !important;
    background: #b63a34 !important;
    color: #ffffff !important;
    text-align: left !important;
  }

  table tr:nth-child(even) td {
    background: #f7f7f7 !important;
  }

  .table-title {
    background: #b63a34;
    color: #ffffff;
    font-weight: 700;
    font-size: 1.45rem;
    line-height: 1.25;
    padding: 12px 14px;
    margin: 2rem 0 0 0;
    border: 1px solid #8f2d28;
  }

  .table-subtitle {
    background: #b63a34;
    color: #ffffff;
    font-weight: 700;
    font-size: 1.08rem;
    line-height: 1.25;
    padding: 10px 14px;
    margin: 1.2rem 0 0 0;
    border: 1px solid #8f2d28;
    border-bottom: 0;
  }

  img {
    max-width: 100%;
    height: auto;
  }
</style>

# Scraping Away Spotted Lanternflies

Deepti Kousik, Jonathan Wan, Jacquelyn Monahan, Brandon Chiang, Jonathan Sacolick

## 1. Context and Problem Statement:

The spotted lanternfly presents an especially challenging problem as its population grows rapidly due to a high number of nymphs surviving to adulthood, where they reproduce abundantly, increasing their population by a factor of 5.47 [1]. Current solutions primarily target adults, but rapid population growth is already occurring by this stage, increasing the severity of their impact regardless.

This aspect is promising as it tackles the root issue: limiting SLF populations by reducing reproduction success. We aim to reduce the overall population of SLFs in a vineyard or region. Creating even a small dent in SLF’s reproduction rate can have a significant impact on their numbers and harm.

## 2. Final Prototype and Application:

Our final prototype is an extendable scraper with a conforming blade that matches the curvature of a surface by utilizing 3-point bending. The scraper is lightweight and has a telescoping handle, allowing it to be used at multiple lengths. The blade is attached to a collection pouch that egg masses fall into when scraped, and the handle itself uses a spring hinge mechanism to vary its angle. Additionally, there are several orientations of the handle, allowing the user to vary its angle with respect to two planes.

The scraper is meant to be an accessible and easy method for users and the general public to scrape egg masses off of trees and other varied surfaces, thus reducing the SLF population and the infestation issue for harvesters. This could be used in vineyards and farms, where SLFs are especially troublesome. Additionally, the scrapers could be incentivized and placed in parks for the general public.

The user workflow is as follows: A user spots an SLF egg mass, extends the scraper using the telescoping handle, scrapes the egg masses using the compliant blade, and finally, the egg masses fall into the collection pouch for easy disposal and removal.

## 3. Conclusion and Recommendation:

This design has potential, but it requires more in-depth updates and field testing. The scraper would be more effective if outfitted with a light, a camera, and a display that would aid users in viewing egg masses, and the telescoping could be automated in future iterations. Our tests proved the scraper could withstand heavy usage and conform to different surfaces, but showed issues with the disposable bag. In the future, the disposable plastic bag should be replaced with a permanent container housing disposable liners, and the scraper should be tested with environmental factors (e.g. weather).

However, even with this design, it is hard to guarantee that people would use the scraper without a larger incentive. Furthermore, it is more expensive than anticipated to implement this, as vineyards would have to hire someone to scrape off the egg masses. More research and studies should be done into existing incentive numbers i.e., how many people use the SLF egg mass credit cards vs how many are handed out. Surveys could be conducted on this to discern if this is truly a promising product. This could affect future implementations of this product, and ways to reduce the production cost should also be considered (whether mass-producing them or switching to certain lower-cost parts).

## 4. Testing and Results:

We aimed to create a scraper that is quick to use, can durably conform to varying surfaces, is comfortable to the average user, and:

- It should be able to be set up and used in under 30 seconds. Time is a high priority.
- It should be able to withstand repeated use, maintaining its functionality by not deforming more than ¼” after 50 times of use. Durability is a high priority.
- It should be able to bend to a minimum radius of curvature of 4 inches to allow it to follow many different surface curvatures for ease of removal. Adapting to different surfaces is a high priority.
- It should require a comfortable level of force for the average user. At least 75% of users must rate their comfort with the force exerted to scrape off ‘egg masses’ at least a 7/10 on flat and curved surfaces. A reasonable comfort level is a high priority.
- It should collect egg masses consistently in the collection pouch. At least 75% of scraped egg masses should fall into the pouch, and it should not overflow or deteriorate within 15 scrapings.

Our earlier prototypes required a lot of force from users despite being able to curve to a large radius, which led us to use a thinner, 1/32” scraper blade. Additionally, we sized up the handle radius to 1-¼”. The final prototype was able to be set up within 15 seconds when replacing the bag (took <5 without replacement), did not show any signs of degradation or deformation after a full exhibition or repeated testing, had a minimum radius of curvature of 9.16”, and was rated highly by users as seen in the chart below. We tested it on trees outside, and it scraped modeled egg masses reasonably well with gravity aiding this, as we struggled to collect our egg masses properly when scraping horizontally during demonstrations. Thus, as seen in this testing, the scraper is easy to set up, durable, conforms to a variety of surfaces, and is comfortable for users.

![Comfort results chart for flat and curved surfaces]({{ "/assets/images/dragonfly/comfort_results_chart.png" | relative_url }})

However, the scraper struggled with collecting egg masses. The disposable pouch only caught egg masses about 50% of the time when tested on trees and seemed flimsy at times. Future iterations of this product should either implement support for the disposable pouch or replace it with a permanent container housing replaceable liners.

## 5. Prototype and Testing Details:

Our first “proof of concept” prototype is shown here and was constructed from cardboard, wood, and paper. This prototype helped us discern estimates for the blade size and handle length and identify problems that arise during physical assembly, such as positioning of the disposable collection pouch.

![Proof of concept prototype]({{ "/assets/images/dragonfly/proof_of_concept_prototype.png" | relative_url }})

We moved from this to our first real prototype, where our main goal was to troubleshoot the scraper blade and test our 3 point bending mechanism, spring hinge, and scraper blade variance. We created CAD as a mockup and constructed the scraper as pictured here. For this prototype, we stress tested it over 40 times to determine if the blade would deflect, had users rate their comfort on flat and curved surfaces with modeled egg masses, and calculated our maximum radius of curvature. The blade experienced negligible deflection, there was no degradation, and the maximum radius of curvature was well above the required 4”. However, users struggled to scrape egg masses on curved surfaces. We also found difficulty in the range of motion with the blade itself, as the spring hinge created a tendency to ‘snap’ back after scraping was done.

| Prototype 1 curved surface test | Prototype 1 blade assembly | Prototype 1 CAD mockup |
|---|---|---|
| ![Prototype 1 curved surface test]({{ "/assets/images/dragonfly/prototype_1_curved_surface_test.png" | relative_url }}) | ![Prototype 1 blade assembly]({{ "/assets/images/dragonfly/prototype_1_blade_assembly.png" | relative_url }}) | ![Prototype 1 CAD mockup]({{ "/assets/images/dragonfly/prototype_1_cad_mockup.png" | relative_url }}) |

Prototype 2 focused on the telescoping handle: making it work, figuring out handle connectors, moving to a new handle size, and testing this. We ordered 2 aluminum hollow rods & 2 different types of handle connectors to determine which was more ideal. Through this, we experimented and found a way to make the rods telescope, and test users unanimously agreed the lever locking mechanism was more intuitive than the knob locking mechanism. We tested the telescoping over 50 uses and saw no degradation during this period.

Our final prototype used a 1/32” CPVC scraper blade, 3 aluminum rods with 2 telescoping connectors, foam to softly stop the scraper blade from ‘snapping’ back, a large disposable bag, lasercut handle connector and triangular handle piece, 3D printer converter to take the circular rod to rectangular to connect to the blade assembly, the same spring hinge, and similar ¼”-20 and M3 hardware. This prototype withstood 50 uses in testing and subsequent use during presentations and exhibition day without significant degradation or deflection, was tested on trees outside, was rated highly across all users on comfort on both curved and flat surfaces, and had a maximum radius of curvature of 9.16”.

![Final prototype exhibit photo]({{ "/assets/images/dragonfly/final_prototype_exhibit_photo.png" | relative_url }})

## 6. Assembly Instructions<sup>1</sup>:

1. Assembling the Scraper Blade
   1. Cut the 1' x 1' CPVC Plate to 4¼" x 2¾" using band saw, belt sand at a 30° angle<sup>1</sup>
   2. Assemble springs onto ¼”-20 bolts and bolt through the laser-cut handle connector and CPVC scraper blade, placing a nut on the other end
      1. Torque the nut to allow for compression while keeping the assembly secure
2. Assembling the Angling Head
   1. Hold the spring hinge open and align it with corresponding holes in the laser-cut pieces
      1. Ensure the hinge folds so the blade goes into the Triangular Handle Piece
   2. Connect to the Handle Connector & Triangular Handle Piece using M3 hardware
   3. Torque nuts tightly with a small wrench
3. Assembling the telescoping handle
   1. Wrap 3 layers of tape on the bottom of the Telescoping Rods to create a makeshift stop
   2. Place the Large Telescoping Connector onto the Large Telescoping Rod
   3. Slide the Medium Rod through the bottom of the Large Rod with the taped side of the Medium one at the bottom (this taped section should not go through the connector)
   4. Using a wrench, tighten the bolts on the Telescoping Connector until the rod can move in it, but there is enough friction to keep hold it when left alone
   5. Repeat for the Small Telescoping Connector and the Small Telescoping Rod
4. Attaching the Angling Head to the handle
   1. Press the 3D Printed Handle Converter onto the Small Telescoping Rod
      1. Holding the blade back to keep it from interfering, align the Triangular Handle Piece and place ¼”-20 bolts through the top and bottom holes (top hole may be chosen by the user and changed anytime to change the orientation of the blade)
      2. Secure with nuts, torque tightly
   2. Be careful not to ‘snap’ the blade in one direction due to the spring hinge
   3. Place foam on top of the Handle Converter as a soft stop for the blade
5. Attach the disposable bag to the back of the blade assembly by pushing it onto the bolts

<sup>1</sup> See “Bill of Materials” - “Final Prototype BOM (and Components List)” for full list of exact components

## References

[1] D. Strömbom and S. Pandey, “Modeling the life cycle of the spotted lanternfly (Lycorma delicatula) with management implications,” Mathematical Biosciences, vol. 340, p. 108670, Jul. 2021, doi: https://doi.org/10.1016/j.mbs.2021.108670.

## Bill of Materials

<div class="table-subtitle">Final Prototype BOM (and Components List)</div>

| Product Name | McMaster Code | Quantity | Total Cost |
|---|---:|---:|---:|
| Spring Hinge Spring Spring Hinge | 15205A83 | One Unit | $1.68 |
| CPVC Scraper Blade High-Temperature CPVC Sheet, 12" x 12" x 1/32" | 8748K21 | One Unit | $10.71 |
| Small Telescoping Connector Lever Locking Connector for 1-3/8" and 1-1/2" OD Light Duty Aluminum Telescoping Rail | 6267N17 | One Unit | $9.24 |
| Large Telescoping Connector Lever Locking Connector for 1-1/4" and 1-3/8" OD Light Duty Aluminum Telescoping Rail | 6267N16 | One Unit | $9.24 |
| Large Telescoping Rod Architectural 6063 Aluminum Round Tube | 6556N111 | One Unit | $17.53 |
| Medium Telescoping Rod Architectural 6063 Aluminum Round Tube | 6556N109 | One Unit | $11.06 |
| Small Telescoping Rod Architectural 6063 Aluminum Round Tube | 6556N108 | One Unit | $10.31 |
| Foam Super-Cushioning Polyurethane Foam Sheet | 8643K491 | One Unit | $18.42 |
| ¼” Acrylic Sheet ¼” Acrylic Sheet for laser cutting | N/A | One Unit | $7.00 |
| Triangular Handle Piece Laser Cut Acrylic | N/A | One Unit | $1.74 (RPL Laser Cutting) |
| Handle Connector Laser Cut Acrylic | N/A | One Unit | $1.09 (RPL Laser Cutting) |
| Handle Converter PLA 3D Print 25.75g | N/A | One Unit | $1.29 |
| ¼”-20 Hardware ¼”-20 Nuts & Bolts | N/A | Free through Taylor Design Studio |  |
| M3 Hardware M3 Nuts & Bolts | N/A | Free through Taylor Design Studio |  |
| **Total:** |  |  | **$99.31** |

<div class="table-subtitle">Overall Project BOM</div>

| Referenced As | Product Name | McMaster Code | Quantity | Total Cost |
|---|---|---:|---:|---:|
| Prototype 1 Handle | Clear Impact-Resistant Polycarbonate Rectangle Tube (1" x 1" x 1') | 3161T31-3161T311 | One Unit | $10.45 |
| Spring Hinge | Spring Hinge | 15205A83 | One Unit | $1.68 |
| Prototype 1 Scraper Blade | 1' x 1' x 1/16" PVC Plate | 8747K111 | One Unit | $4.71 |
| CPVC Scraper Blade | High-Temperature CPVC Sheet, 12" x 12" x 1/32" | 8748K21 | One Unit | $10.71 |
| Large Telescoping Connector | Lever Locking Connector for 1-3/8" and 1-1/2" OD Light Duty Aluminum Telescoping Rail | 6267N17 | One Unit | $9.24 |
| Small Telescoping Connector | Lever Locking Connector for 1-1/4" and 1-3/8" OD Light Duty Aluminum Telescoping Rail | 6267N16 | One Unit | $9.24 |
| Prototype 2 Telescoping Connector | Knob Locking Connector for 1-3/8" and 1-1/2" OD Light Duty Aluminum Telescoping Rail | 6267N25 | One Unit | $9.16 |
| Large Telescoping Rod | Architectural 6063 Aluminum Round Tube | 6556N111 | One Unit | $17.53 |
| Medium Telescoping Rod | Architectural 6063 Aluminum Round Tube | 6556N109 | One Unit | $11.06 |
| Small Telescoping Rod | Architectural 6063 Aluminum Round Tube | 6556N108 | One Unit | $10.31 |
| Foam | Super-Cushioning Polyurethane Foam Sheet | 8643K491 | One Unit | $18.42 |
| ¼” Acrylic Sheet | ¼” Acrylic Sheet for laser cutting | N/A | One Unit | $7.00 |
| Triangular Handle Piece | Laser Cut ¼” Acrylic | N/A | One Unit | $1.74 (RPL Laser Cutting) |
| Handle Connector | Laser Cut ¼” Acrylic | N/A | One Unit | $1.09 (RPL Laser Cutting) |
| Handle Converter | PLA 3D Print 25.75g | N/A | One Unit | $1.29 |
| ¼”-20 Hardware | ¼”-20 Nuts & Bolts | N/A | Free through Taylor Design Studio |  |
| M3 Hardware | M3 Nuts & Bolts | N/A | Free through Taylor Design Studio |  |
| **Total:** |  |  |  | **$123.63** |

## Response to Absences:

During the week of 4/06, two of our members, Jonathan and Jonathan, were unable to attend the lab session. Due to these being previously mentioned and excused absences, they were given tasks to do asynchronously, CADing and 3D printing an Adapter, and were updated through our group chat and at the next lab session.
