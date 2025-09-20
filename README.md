## name: n v mohana krishna
## reg: 212224100039
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


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report

<img width="1372" height="996" alt="image" src="https://github.com/user-attachments/assets/78183887-fa1e-4d41-aa7a-0bdad5686a4c" />

<img width="1725" height="1094" alt="Screenshot 2025-09-20 144127" src="https://github.com/user-attachments/assets/5e06ec2b-5aa5-43c6-878d-844808f61171" />

<img width="1072" height="670" alt="Screenshot 2025-09-20 144949" src="https://github.com/user-attachments/assets/162a9895-ad81-4fa1-82b6-905dd44c166c" />

<img width="1070" height="667" alt="Screenshot 2025-09-20 145009" src="https://github.com/user-attachments/assets/6e2a5ea9-5256-4efe-bce7-99b897caf208" />

<img width="1709" height="1067" alt="Screenshot 2025-09-20 145049" src="https://github.com/user-attachments/assets/c8ccbce3-6a40-409a-b350-8fd06c3cced8" />

<img width="1711" height="1066" alt="Screenshot 2025-09-20 145121" src="https://github.com/user-attachments/assets/9fef6c25-1f45-44c2-b603-52b56818ea00" />

<img width="1905" height="1199" alt="Screenshot 2025-09-20 145030" src="https://github.com/user-attachments/assets/bf9f59b1-cd8d-4b29-bed7-172f7a8fe246" />


## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

