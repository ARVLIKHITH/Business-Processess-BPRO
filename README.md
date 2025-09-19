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

---

## BPMN (Process Modelling with Camunda)

The first part of the project focused on **Business Process Modelling** using **BPMN (Business Process Model and Notation)**.  
The task was to **design a digital schema** that outlines every key step in the lifecycle of the product – from **procurement of raw materials** to **final customer delivery**.  

I used **Camunda Modeler** to build the BPMN diagram, and I also created a **Process Profile** (document) that defined all the process inputs, outputs, suppliers, and customers.  

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
- `docs/BPMN_Schema.png` → BPMN schema created with Camunda Modeler.
- <img width="13986" height="10272" alt="BPMN Schema (HDPE Pipe)" src="https://github.com/user-attachments/assets/bc472a0a-0782-4aed-915d-e94da5b86241" />
  
- ' ' → Proposed process improvements to further optimise production workflows and minimise material waste.
