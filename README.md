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

<img width="944" height="453" alt="image" src="https://github.com/user-attachments/assets/da8198c3-88f8-40c9-b581-d4545b7fd62f" />

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

### Routings – Example (HDPE Pipe)

| Operation | Work Center | Description     | Control Key | Setup (min) | Labor (min) |
|-----------|-------------|-----------------|-------------|-------------|-------------|
| 0010      | BA-PQ-0G    | Packaging       | PP01        | 3           | 2           |
| 0020      | BA-QU-0G    | Quality Check   | PP01        | 5           | 5           |
| 0030      | BA-LA-0G    | Labelling       | PP01        | 3           | 2           |
| 0040      | BA-PR-0G    | Processing      | PP03        | 3           | -           |

---

### Costing & Price Updates

| Product            | Estimated Cost (€) | Price Released |
|--------------------|--------------------|----------------|
| HDPE Pipe (FP)     | 20.65 / unit       | ✔              |
| Mixture (SF)       | Updated            | ✔              |
| Heated Pipe (SF)   | Updated            | ✔              |
| Printed Pipe (SF)  | Updated            | ✔              |

---

### Confirmations & Production Orders

- Generated and confirmed **80+ production order confirmations**.  
- Used **CO11N** to enter time tickets for each routing step.  
- Adjusted planned vs actual times for realistic confirmation data.  
- Linked production orders with **Goods Issues (GI)** and **Goods Receipts (GR)**.  

---

## SAP Outcome

- Demonstrated **end-to-end ERP integration** inside SAP.  
- Validated the complete flow: **procurement → production → sales → costing → inventory → invoicing**.  
- Achieved required **80+ confirmations**, proving process reliability.  

---



