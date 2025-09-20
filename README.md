# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


<img width="944" height="746" alt="Screenshot 2025-09-20 140514" src="https://github.com/user-attachments/assets/5075b4de-599d-4a93-a762-336d61778fd0" />

<img width="1095" height="720" alt="Screenshot 2025-09-20 at 8 39 08 PM" src="https://github.com/user-attachments/assets/240c36e7-18fd-413f-b224-d6935150d39d" />

<img width="1556" height="795" alt="Screenshot 2025-09-20 at 8 39 27 PM" src="https://github.com/user-attachments/assets/28db7c36-e0da-4949-b745-f27eb82d54ec" />

<img width="1548" height="757" alt="Screenshot 2025-09-20 at 8 39 51 PM" src="https://github.com/user-attachments/assets/fa621355-b56a-4041-8f7c-78c6cce13cab" />

<img width="1115" height="567" alt="Screenshot 2025-09-20 at 8 40 15 PM" src="https://github.com/user-attachments/assets/fecc8ee2-71ed-4661-986c-eb834209365c" />

<img width="871" height="551" alt="Screenshot 2025-09-20 at 8 41 03 PM" src="https://github.com/user-attachments/assets/5d7de799-8fe0-436e-ad46-0e99e0ae42cc" />

<img width="1511" height="617" alt="Screenshot 2025-09-20 at 8 41 20 PM" src="https://github.com/user-attachments/assets/b6315efc-ed62-4d93-b507-1968f697f61f" />

<img width="716" height="712" alt="Screenshot 2025-09-20 at 8 41 36 PM" src="https://github.com/user-attachments/assets/b01ba811-571b-4146-892c-f4b48e2d37c7" />

## OUTPUT:
Unallocated Space Analysis and Extracted Data Report

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

