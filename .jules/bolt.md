## 2025-05-14 - Initial Analysis of Emotion Analysis Notebook
**Learning:** Found a classic performance anti-pattern in a Jupyter Notebook: reading and writing the entire results CSV file inside a loop ((N^2)$ I/O). This is a major bottleneck as the number of processed images increases.
**Action:** Replace the full CSV read/write with a direct append mode (`mode='a'`) to the CSV file, which is (1)$ per iteration.
