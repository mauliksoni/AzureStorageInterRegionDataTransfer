# Azure Storage Accounts Inter region data transfer speed test

Test Case 1
| Type | Source Storage Account  | Destination Storage Account | Size | # of Files | Copy Method | VM |
|---|---|---|---|---|---|---|
| ADLS Gen 2 Standard No Hierarchical namespace | Canada Central | East US 2 | 10 GiB | 1 | az copy | D8ads_v5 (8 CPU x 32 Gib Memory) Win 11 Canada Central |

100 GiB file is created using fsutil file createnew c:\temp\a.bin 1048576000000

Results

| Upload to Canda Central from Canada Central | Transfer from Canada Central to US East 2 |
|---|---|
| Avg 4000 Mbps  | Avg 5500 Mbps  |
| 195 Seconds | 198 Seconds |
