# Answers

## To-do1

### to-do1-1
**Meaning of columns:**
- **si (Swap In):** Amount of memory swapped in from disk (/s).
- **so (Swap Out):** Amount of memory swapped to disk (/s).
- **bi (Blocks In):** Blocks received from a block device (blocks/s).
- **bo (Blocks Out):** Blocks sent to a block device (blocks/s).

*(Note: `vmstat` command was not available in the environment, so no output file was generated.)*

## To-do2

### to-do2-1 (First Fit)
| Process | Starting Address | Ending Address |
| :--- | :--- | :--- |
| P1 | | |
| P2 | | |
| P3 | | |
| P4 | | |

### to-do2-2 (Best Fit)
| Process | Starting Address | Ending Address |
| :--- | :--- | :--- |
| P1 | | |
| P2 | | |
| P3 | | |
| P4 | | |

### to-do2-3
**Issues:**
- **First Fit:** May break large blocks of memory into smaller fragments at the beginning, potentially preventing larger processes from finding space later.
- **Best Fit:** Creates very small fragments (external fragmentation) that are too small to be useful for any process.
- **General:** Both suffer from external fragmentation. P3 and P4 might not fit if fragmentation is high.

## To-do3

### to-do3-1
**Number of memory frames:**
- Total RAM = 16 TB = $16 \times 2^{40}$ bytes = $2^4 \times 2^{40} = 2^{44}$ bytes.
- Page Size = 4 KB = $4 \times 2^{10} = 2^{12}$ bytes.
- Number of Frames = Total RAM / Page Size = $2^{44} / 2^{12} = 2^{32}$ frames (approx 4.29 billion).

### to-do3-2
**Bits for displacement (offset):**
- Page Size = 4 KB = $2^{12}$ bytes.
- Displacement bits = $\log_2(2^{12}) = 12$ bits.

### to-do3-3
**Virtual Memory Size:**
- Index bits (p) = 36.
- Offset bits (d) = 12.
- Total logical address bits = $36 + 12 = 48$ bits.
- Virtual Memory Size = $2^{48}$ bytes = 256 TB.