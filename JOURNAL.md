## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/149

**Issue title:** Structural chunker silently drops documents that contain no headings 

**Tier:**  Tier 1

**Problem summary:**
The issue is that the structural chunker returns an empty list when the document is missing a heading. The thing that is missing is a path to handle when a document doesn't have a header so that it can still be chunked. A successful fix would have another condition to extract text that doesn't rely upon headings to split the text. The problem is located in ingestion/chunking/structural_chunker.py

**Is this right for me** 
The structural chunker isn't properly chunking text without headers. 
The ingestion is what is being affected
The app should properly chunk text without a header.

This is my first open source contribution, and the issue is tier 1

I have found the relavent code
I understand the file well enough that I can change it.
I have read the relavent file test.

I am fine with how many other people are on this issue.
I am confident I can complete this before the week 9 deadline.
This issue has no blockers or dependencies.
**Branch name:** fix/149-structural-chunker-drops-documents

**Setup confirmation:** ![alt text](image.png) App runs locally at localhost:5173

**Cohort ledger:** Issue added to cohort ledger