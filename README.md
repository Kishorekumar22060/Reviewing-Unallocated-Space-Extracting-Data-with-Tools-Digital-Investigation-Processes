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

<img width="1920" height="1080" alt="Screenshot 2025-09-20 140545" src="https://github.com/user-attachments/assets/0dc4a16d-6087-418a-bcc1-a793ec08c70e" />


<img width="1920" height="1080" alt="Screenshot 2025-09-20 140604" src="https://github.com/user-attachments/assets/df722e77-4be8-4eec-aea2-13ff8c821bb8" />

<img width="1920" height="1080" alt="Screenshot 2025-09-20 140807" src="https://github.com/user-attachments/assets/713dfb4b-0f34-4f81-8d39-b9a4c539f2a5" />


<img width="1920" height="1080" alt="Screenshot 2025-09-20 141708" src="https://github.com/user-attachments/assets/073e3188-196a-49b3-bf09-1e31851b23ab" />



<img width="1920" height="1080" alt="Screenshot 2025-09-20 142224" src="https://github.com/user-attachments/assets/3730692c-d571-4c1c-ba2f-9b456d6d7072" />

<img width="1920" height="1080" alt="Screenshot 2025-09-20 142307" src="https://github.com/user-attachments/assets/06253722-6c7e-488a-a089-e61836836fa1" />



<img width="1920" height="1080" alt="Screenshot 2025-09-20 142336" src="https://github.com/user-attachments/assets/606a8fc7-ae5c-4493-afa9-38e2254797ac" />

<img width="1920" height="1080" alt="Screenshot 2025-09-20 142526" src="https://github.com/user-attachments/assets/4f34846d-3131-47b0-9bb0-371a385cf136" />

<img width="1920" height="1080" alt="Screenshot 2025-09-20 143418" src="https://github.com/user-attachments/assets/7bab635b-135d-4f5d-a106-5a2d8bd15a1d" />



## OUTPUT:
Unallocated Space Analysis and Extracted Data Report

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

