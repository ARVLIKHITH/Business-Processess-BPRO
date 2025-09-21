# Business Processes & ERP Simulation (BPRO Project)

This repository documents my **BPRO (Business Processes) project**, where the main objective was to **simulate the entire lifecycle of a product** in three different ways:  

1. **BPMN Schema** – Modelling the process flow of the company  
2. **AP Plus ERP** – Structuring master data and simulating digital manufacturing  
3. **SAP S/4HANA** – Executing the same processes across multiple integrated ERP modules  

The project was designed to bridge **business understanding and technical ERP execution**. This project was carried out as part of the BPRO module under the guidance of Technische Hochschule Würzburg-Schweinfurt (FHWS) faculty. 
We were required to contact a Manufacturing company, obtain real data about one product, and then transform this into digital processes across the platforms.  

---

## Project Assignment & Structure

- **Step 1 (Company Contact):** Approach a Manufacturing company and select one product.  
- **Step 2 (Data Collection):** Gather process-related data, including raw materials, production stages and procurement details.  
- **Step 3 (BPMN):** Model the entire product lifecycle digitally using BPMN.  
- **Step 4 (APplus ERP):** Enter the master data, create routings, simulate orders, and compare costs digitally.  
- **Step 5 (SAP S/4HANA):** Rebuild the same data and processes inside SAP across MM, PP, WM, and FI modules.  

This ensured that we didn’t just learn ERP software but also understood **how businesses actually run their operations** and how ERP captures that in a structured way.  

---

## Company Background – Vahini Pipes

I collaborated with **[Vahini Irrigation Pvt. Ltd.](https://vahinipipes.com/)**, a manufacturing company in India that specialises in **HDPE pipes for irrigation and water systems**.  

- **Industry:** Manufacturing & Irrigation Systems  
- **Technology Used:** Extrusion, Cooling, Cutting, Packaging, Quality Testing  
- **Chosen Product:** **HDPE Pipe**  
- **Reason for Selection:**  
  - Full supply chain involvement (raw materials → extrusion & machining → packaging → quality → delivery).  
  - Offers complexity in procurement and production, making it ideal for ERP modelling.  

This company context provided a **real foundation** to carry the product data across BPMN, AP Plus, and SAP.

<p align="center">
  <img src="https://github.com/user-attachments/assets/da8198c3-88f8-40c9-b581-d4545b7fd62f" alt="Robodroid Prototype" width="900"/>
</p>
---

## Bill Of Materials

![Screenshot_20-9-2025_173155_](https://github.com/user-attachments/assets/13d286dc-d69b-4b2d-9c0d-cd92bfd33ec5)

---

## BPMN (Process Modelling with Camunda)

The first part of the project focused on **Business Process Modelling** using **BPMN (Business Process Model and Notation)**.  
The task was to **design a digital schema** that outlines every key step in the lifecycle of the product – from **procurement of raw materials** to **final customer delivery**.  

I used **Camunda Modeller** to build the BPMN diagram, and I also created a **Process Profile** (document) that defined all the process inputs, outputs, suppliers, and customers.  

---

### Subsection 1: Story of BPMN Work

- **Objective:** Model the real-life processes of Vahini Pipes digitally.  
- **Approach:**  
  - Identified all raw materials and suppliers.  
  - Mapped out each production stage (Extrusion, Cooling, Cutting, Packaging, Quality, Labelling, Processing).  
  - Added procurement processes (purchase orders, goods receipt, invoice verification).  
  - Added sales processes (customer orders, deliveries, invoicing).  
- **Outcome:**  
  - A complete **BPMN schema** was developed.  
  - It represented the **end-to-end integration of procurement, production, quality, warehousing, and customer delivery**.  
  - Supported by a **Process Profile** with performance metrics (time, yield, costs, customer satisfaction).  

This was the **foundation of the BPRO project**, ensuring the rest of the work in APplus and SAP followed the same logic.  

---

### Subsection 2: Process Profile & BPMN Schema

📂 Files included:  
- 📂 [Process Profile Report (PDF)](./Process%20Profile.pdf) → Full Process Profile (inputs, outputs, suppliers, customers, metrics).  
- 📂 BPMN schema created with Camunda Modeller.
  
 ![BPMN Schema](./BPMN%20Schema%20(HDPE%20Pipe).png) 
 
- 📂 [Process Improvement Presentation (PDF)](./Process%20Improvement.pdf) → Proposed process improvements to further optimise production workflows and minimise material waste.
  
---

# AP Plus ERP

The second part of the BPRO project focused on **APplus ERP**, where I digitally structured and simulated the production of HDPE pipes.  

This phase emphasised **master data creation, order management, costing, and machine scheduling**.  
Unlike SAP, APplus is designed to show process data in a more **visual and planning-oriented way**, with Gantt charts and efficiency targets.  

---

## Story of AP Plus Work

- **Objective:** Build the digital backbone of the company (Vahini Pipes) by entering all **master data** and simulating its operations.  
- **Approach:**  
  - Created all **materials, BOMs, routings, work centres, and machines**.  
  - Structured **customer master data, vendor data, and pricing**.  
  - Entered multiple **customer orders** and triggered procurement for raw materials.  
  - Monitored digital manufacturing flow through APplus dashboards.  
  - Analysed **planned vs. target cost** to track efficiency.  
- **Challenge:**  
  - At the end of the project, all machines had to reach **80% utilisation**.  
  - To achieve this, I carefully scheduled orders in the **Gantt chart**, balancing workloads and timing to ensure each machine reached the 80% efficiency threshold.  
- **Outcome:**  
  -  Achieved machine utilisation targets across all work centres.
    

   <img width="1377" height="562" alt="Screenshot 2025-01-18 at 6 42 38 PM" src="https://github.com/user-attachments/assets/c7fcb061-66ed-4cf1-b247-e005c5a77e94" />
   
   
  -  Demonstrated Comparative costing for the final product with the customer order AB1000002.
   
    
  <img width="1107" height="784" alt="Screenshot 2025-01-17 at 5 06 29 AM copy" src="https://github.com/user-attachments/assets/7971bf5b-e16f-4935-ba87-b53d62f104bf" />
  
  
----

## SAP S/4HANA

The third and final part of the BPRO project involved executing the processes in **SAP S/4HANA**.  
This part was more advanced, as I had to work across **multiple integrated modules**:  

- **MM (Materials Management)** – Vendors, purchase orders, invoice verification  
- **PP (Production Planning)** – BOM, routings, work centers, production orders  
- **WM (Warehouse Management)** – Goods receipts, goods issues, storage locations  
- **FI (Financial Accounting)** – Invoices, payments, and financial postings  

---

### Story of SAP Work

After structuring data in APplus, the same logic was replicated in SAP.  
I created all relevant master data, processed procurement, and ran the complete **sales-to-billing cycle**.  

- **Challenge:** Instead of machine utilisation like in APplus, here I had to achieve **80+ confirmations**, one generated from each routing.  
- Result: Successfully completed more than **80 confirmations**, ensuring that production, routing, and costing processes were validated.
  
---

### Material Master Data

| Material Code  | Description              | Type            | UoM | Plant |
|----------------|--------------------------|-----------------|-----|-------|
| BPA-HDPEP-0G   | HDPE Pipe (Finished)    | Finished Good   | PC  | 1000  |
| BPA-HACSP-0G   | Heated & Cooled Pipe    | Semi-Finished   | PC  | 1000  |
| BPA-CUTSP-0G   | Cut Pipe                | Semi-Finished   | PC  | 1000  |
| BPA-MIXTU-0G   | Mixture                 | Semi-Finished   | KG  | 1000  |
| BPA-PRISP-0G   | Printed Pipe            | Semi-Finished   | KG  | 1000  |
| BPA-PACSP-0G   | Package                 | Semi-Finished   | KG  | 1000  |
| BPA-RESIN-0G   | Resin H829              | Raw Material    | KG  | 1000  |
| BPA-TITAN-0G   | Titanium                | Raw Material    | KG  | 1000  |
| BPA-UVRMP-0G   | UV Stabiliser           | Raw Material    | KG  | 1000  |
| BPA-WAXIS-0G   | 629 Wax Inner Surface   | Raw Material    | KG  | 1000  |
| BPA-WAXOS-0G   | 4201/629 Wax Outer      | Raw Material    | KG  | 1000  |
| BPA-PAPER-0G   | Paper                   | Raw Material    | KG  | 1000  |
| BPA-PLAST-0G   | Plastic                 | Raw Material    | KG  | 1000  |
| BPA-INKPP-0G   | Ink                     | Raw Material    | KG  | 1000  |
| BPA-ACRYL-0G   | Acrylic Resin           | Raw Material    | KG  | 1000  |
| BPA-OILPP-0G   | 120 Oil                 | Raw Material    | KG  | 1000  |
| BPA-IMPFM-0G   | Impact Modifier FM50    | Raw Material    | KG  | 1000  |
| BPA-IMPMB-0G   | Impact Modifier B564    | Raw Material    | KG  | 1000  |
| BPA-PKACH-0G   | PK7 Kaneka Chemical     | Raw Material    | KG  | 1000  |
| BPA-WATER-0G   | Water                   | Raw Material    | KG  | 1000  |

### Bill of Materials (BOM)

| Parent Product   | Component Material | Quantity | UoM | Notes                        |
|------------------|--------------------|----------|-----|------------------------------|
| **BPA-HDPEP-0G** (HDPE Pipe, Finished) | BPA-HACSP-0G (Heated & Cooled Pipe) | 1 | PC  | Semi-Finished |
|                  | BPA-CUTSP-0G (Cut Pipe)           | 1 | PC  | Semi-Finished |
|                  | BPA-PRISP-0G (Printed Pipe)       | 1 | KG  | Semi-Finished |
|                  | BPA-PACSP-0G (Package)            | 1 | KG  | Semi-Finished |
| **BPA-MIXTU-0G** (Mixture, Semi-Finished) | BPA-RESIN-0G (Resin H829)        | 9.5  | KG  | Raw Material |
|                  | BPA-IMPFM-0G (Impact Modifier FM50) | 0.3  | KG  | Raw Material |
|                  | BPA-IMPMB-0G (Impact Modifier B564) | 0.1  | KG  | Raw Material |
|                  | BPA-PKACH-0G (PK7 Kaneka Chemical) | 0.3  | KG  | Raw Material |
|                  | BPA-TITAN-0G (Titanium)            | 0.6  | KG  | Raw Material |
|                  | BPA-WAXIS-0G (Wax Inner Surface)   | 0.3  | KG  | Raw Material |
|                  | BPA-WAXOS-0G (Wax Outer Surface)   | 0.3  | KG  | Raw Material |
|                  | BPA-OILPP-0G (120 Oil)             | 0.2  | KG  | Raw Material |
|                  | BPA-WATER-0G (Water)               | 50   | KG  | Raw Material |
| **BPA-PRISP-0G** (Printed Pipe, Semi-Finished) | BPA-INKPP-0G (Ink)              | 0.2  | KG  | Raw Material |
|                  | BPA-ACRYL-0G (Acrylic Resin)       | 0.2  | KG  | Raw Material |
|                  | BPA-WATER-0G (Water)               | 50   | KG  | Raw Material |
| **BPA-PACSP-0G** (Package, Semi-Finished) | BPA-PLAST-0G (Plastic)           | 0.2  | KG  | Raw Material |

### Work Centres

| Work Center | Description       | Plant | Control Key | Notes                       |
|-------------|-------------------|-------|-------------|-----------------------------|
| BA-EX-0G    | Extrusion         | 1000  | PP01        | Core pipe forming process   |
| BA-CC-0G    | Cooling           | 1000  | PP01        | Post-extrusion cooling      |
| BA-AE-0G    | Aeration          | 1000  | PP03        | Air treatment               |
| BA-CU-0G    | Cutting           | 1000  | PP01        | Pipe cutting                |
| BA-GR-0G    | Grinding          | 1000  | PP03        | Surface finishing           |
| BA-PQ-0G    | Packaging         | 1000  | PP01        | Packaging for delivery      |
| BA-QU-0G    | Quality Check     | 1000  | PP01        | Inspection & testing        |
| BA-LA-0G    | Labelling         | 1000  | PP01        | Product identification      |
| BA-PR-0G    | Processing        | 1000  | PP03        | Final processing step       |
| BA-MI-0G    | Mixing            | 1000  | PP01        | Raw material mixing         |
| BA-WI-0G    | Weighing          | 1000  | PP01        | Weight verification         |
| BA-PO-0G    | Pouring           | 1000  | PP03        | Material pouring            |
| BA-CO-0G    | Combining         | 1000  | PP01        | Blend combination           |
| BA-AD-0G    | Adding            | 1000  | PP03        | Additives input             |
| BA-IN-0G    | Ink Formulation   | 1000  | PP01        | Ink & resin preparation     |
| BA-BL-0G    | Blending          | 1000  | PP03        | Final material blending     |

---

### Sample Routing (HDPE Pipe)

| Operation | Work Center | Description    | Control Key | Setup (min) | Labor (min) |
|-----------|-------------|----------------|-------------|-------------|-------------|
| 0010      | BA-EX-0G    | Extrusion      | PP01        | 4           | 4           |
| 0020      | BA-CC-0G    | Cooling        | PP01        | 4           | -           |
| 0030      | BA-AE-0G    | Aeration       | PP03        | 2           | -           |
| 0040      | BA-CU-0G    | Cutting        | PP01        | 6           | 6           |
| 0050      | BA-GR-0G    | Grinding       | PP03        | 4           | 4           |
| 0060      | BA-PQ-0G    | Packaging      | PP01        | 3           | 2           |
| 0070      | BA-QU-0G    | Quality Check  | PP01        | 5           | 5           |
| 0080      | BA-LA-0G    | Labelling      | PP01        | 3           | 2           |
| 0090      | BA-PR-0G    | Processing     | PP03        | 3           | -           |

### Customer Master Data

| Customer Code | Customer Name               | Location (DE)      | Notes                          |
|---------------|-----------------------------|--------------------|--------------------------------|
| BPA-CU01-0G   | Rohr GMBH                   | Frankfurt          | Major distributor, bulk orders |
| BPA-CU02-0G   | BAUG                        | Munich             | Construction industry client   |
| BPA-CU03-0G   | Rhoen-Grabfeld Maustechnik  | Schweinfurt        | Regional SME                   |
| BPA-CU04-0G   | Tech GMBH                   | Nuremberg          | Engineering/industrial client  |
| BPA-CU05-0G   | Mahalakshmi Pvt. Ltd        | Stuttgart          | International partner (subsidiary in DE) |
| BPA-CU06-0G   | Studentenwerk PVT           | Würzburg           | Institutional customer         |
| BPA-CU07-0G   | Mainfranken Installationen  | Würzburg           | Local contractor               |
| BPA-CU08-0G   | Ledward PVT. Ltd            | Berlin             | Urban utility projects         |
| BPA-CU09-0G   | Pasadena PVT. Ltd           | Hamburg            | Long-term contract client      |

### Vendor Master Data

| Vendor Code  | Supplier Name          | Location (DE) | Material Supplied        |
|--------------|------------------------|---------------|--------------------------|
| BPA-VAQ-0G   | Rishabh Texim LPP-GJ   | Hamburg       | Paper, Packaging         |
| BPA-VSI-0G   | Silvin Additives       | Frankfurt     | Titanium, UV stabilisers |
| BPA-VBA-0G   | Basil Prompt Vinyl PVT | Stuttgart     | Wax (Inner & Outer)      |
| BPA-VRI-0G   | Resin Supply Intl.     | Munich        | Resin H829               |
| BPA-VIN-0G   | Ink Pack GMBH          | Berlin        | Printing Ink             |
| BPA-VPM-0G   | Pac Mate GMBH          | Cologne       | Plastic, Packaging       |
| BPA-VAU-0G   | Aqua Supply GMBH       | Bremen        | Water & additives        |

### Sales Price (Finished Product)

------------------------------
Sales Org.     1000                FHWS Sales SW
Distr. Channel 00                  Stand.distr.channel
|Material                                                           |
|CnTy ReSt S Scale Qty UoM Amount Unit per UoM Valid From Valid To  |
|BPA-HDPEP-0G                                                       |
|PR00                      20,65  EUR   1  PC  15.01.2025 31.12.2026|

---------------------------------------------------------------------     

### Costing & Price Updates

| Product            | Estimated Cost (€) | Price Released |
|--------------------|--------------------|----------------|
| HDPE Pipe (FP)     | 20.65 / unit       | ✔              |
| Mixture (SF)       | Updated            | ✔              |
| Heated Pipe (SF)   | Updated            | ✔              |
| Printed Pipe (SF)  | Updated            | ✔              |

### Procurement – Sample Purchase Orders

| Purchase Doc | Supplier   | Material            | Qty   | Net Value (€) |
|--------------|------------|---------------------|-------|---------------|
| 4500001947   | BPA-VAQ-0G | Paper 0G            | 0.2kg | 4.00          |
| 4500001950   | BPA-VBA-0G | 629 Wax Inner       | 0.3kg | 4.50          |
| 4500001951   | BPA-VBA-0G | UV 0G               | 0.4kg | 9.00          |
| 4500001955   | BPA-VRI-0G | Resin H829 0G       | 9.5kg | 29.93         |
| 4500001957   | BPA-VSI-0G | Titanium 0G         | 0.6kg | 8.00          |

**Summary:** Over **50+ purchase orders** were created for suppliers, covering raw materials such as resin, wax, titanium, modifiers, water, and other additives.

---

### Sales – Customer Invoices

| Customer             | Document No | Type | Value (€) |
|----------------------|-------------|------|-----------|
| Rohr GMBH            | 90000389    | RV   | 245.74    |
| BAUG                 | 90000402    | RV   | 737.21    |
| Rhon-Grabfeld        | 90000404    | RV   | 491.47    |
| Tech GMBH            | 90000416    | RV   | 1,228.68  |
| Mahalakshmi Pvt. Ltd | 90000566    | RV   | 1,351.54  |
| Studentenwerk PVT    | 90000565    | RV   | 860.07    |

**Summary:** Invoices generated for **10+ customers**, with a combined sales value of more than **€4,900**.

---

### Costing & Price Updates

| Product            | Estimated Cost (€) | Price Released |
|--------------------|--------------------|----------------|
| HDPE Pipe (FP)     | 20.65 / unit       | ✔              |
| Mixture (SF)       | Updated            | ✔              |
| Heated Pipe (SF)   | Updated            | ✔              |
| Printed Pipe (SF)  | Updated            | ✔              |

**Created Cost Estimates**  
   - Based on **BOM + Routings + Work Centers**.  
   - Included material cost, labour cost, and overheads. 

### Sample Cost Estimate Table

| Product            | Estimated Cost (€) | Released as Standard Price |
|--------------------|--------------------|----------------------------|
| BPA-HDPEP-0G (HDPE Pipe, FG) | 20.65 / unit       | ✔                          |
| BPA-MIXTU-0G (Mixture, SF)   | 8.30 / unit        | ✔                          |
| BPA-HACSP-0G (Heated Pipe, SF)| 5.25 / unit        | ✔                          |
| BPA-PRISP-0G (Printed Pipe, SF)| 4.80 / unit       | ✔                          |
| BPA-PACSP-0G (Package, SF)    | 2.10 / unit        | ✔                          |

**Summary:**

- The **finished HDPE Pipe** had a final cost of **€20.65 per unit**.  
- Semi-finished assemblies were also costed individually and updated in the system.  
- Variance analysis showed that machine utilisation and order scheduling strongly influenced costs.  
- With price release, the updated costs flowed into **sales orders, invoices, and profitability reports**.  

---

### Confirmations & Production Orders

- Generated and confirmed **80+ production order confirmations**.  
- Used **CO11N** to enter time tickets for each routing step.  
- Adjusted planned vs actual times for realistic confirmation data.  
- Linked production orders with **Goods Issues (GI)** and **Goods Receipts (GR)**.
  
**Summary:**

- Each routing step in production required a **confirmation**.  
- Confirmations validated the execution of:  
  - Setup time  
  - Processing time  
  - Labour time  
  - Goods issues/receipts
    
In SAP:  
- Focus was on **number of confirmations**.  
- Target: At least **80 confirmations** (1 per routing step).  
- Completed **125 confirmations** successfully.  

### Sample Confirmations Log (SAP S/4HANA)

| Production Order | Operation | Work Center | Confirmation No | Status    |
|------------------|-----------|-------------|-----------------|-----------|
| 1000001          | 0010      | BA-EX-0G    | C0001           | Confirmed |
| 1000001          | 0020      | BA-CC-0G    | C0002           | Confirmed |
| 1000001          | 0030      | BA-AE-0G    | C0003           | Confirmed |
| 1000001          | 0040      | BA-CU-0G    | C0004           | Confirmed |
| 1000002          | 0010      | BA-MI-0G    | C0005           | Confirmed |
| 1000002          | 0020      | BA-WI-0G    | C0006           | Confirmed |
| 1000002          | 0030      | BA-PO-0G    | C0007           | Confirmed |

---
## SAP Outcome

- Demonstrated **end-to-end ERP integration** inside SAP.  
- Validated the complete flow: **procurement → production → sales → costing → inventory → invoicing**.  
- Achieved required **80+ confirmations**, proving process reliability.  

---
## License  

This repository is shared **for viewing purposes only**.  
All rights reserved © 2025 Likhith Anand.  

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)  

- No copying, reproduction, modification, or redistribution of the content is permitted.  
- All SAP system interfaces, outputs, and screenshots are **© SAP SE**.  
- The academic coursework framework is **© FHWS**.  
- Only my **own contributions** (master data entries, BPMN diagrams, tables, analysis) are included here for demonstration.  

---

---
## Disclaimer  

This repository contains a **public summary** of my academic project in SAP S/4HANA (BPRO Module).  

- All SAP system interfaces, outputs, and screenshots are **© SAP SE**.  
- The academic coursework framework is **© Technische Hochschule Würzburg-Schweinfurt (FHWS)**.  
- Only my **own contributions** (master data entries, process design, BPMN diagrams, tables, and analysis) are included here.  
- The **full project report** with detailed SAP screenshots and proprietary content is **not published publicly**.  

📂 **Full SAP Project Report – Request Access**  
The complete report is available **only upon request for interview or academic review purposes**.  
Please request access via **Google Drive** or contact me directly.  





