# PDM Vault Queries

As a SOLIDWORKS PDM specialist, there are questions about vault health and user behavior that are not easily answered directly within the PDM application interface. 
These queries hit the underlying SQL Server database to answer these questions.
This will be a growing list as customer issues arise. 

---

## Queries

| Query | Description |
|---|---|
| **Files Stuck in Workflow** | Identifies files that have been in the same workflow state longer than a defined threshold. |
| **Duplicate Files** | Identifies filenames that appear more than once across non-deleted documents. |
| **Version Count by File** | Ranks files by number of versions, highest first. Includes file path to distinguish same-named files in different vault locations. |
| **Least Used States and Transitions** | Ranks workflow states and transitions by usage frequency. Useful for identifying cleanup candidates. |
| **User Check-in Activity** | Ranks active users by check-in count per month. |
| **Days to Complete Workflow Cycle** | Calculates how long files take to move from first transition to a defined end state. |
| **Long-Term Checkouts** | Identifies users holding checkouts beyond a defined threshold, with file count and longest duration. |

---

## Environment

- Written using **SQL Server 2025 Standard (Developer)** on **Windows Server 2025**

**Tested on:**
- Two production PDM customer databases

---

## AI Usage Disclaimer

- No AI was used to write these queries.
