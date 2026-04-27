# SCL-180nm-Standard-Cell-Library-Expansion-Drive-Strength-Optimization

**Target Node**: 180nm Bulk CMOS (SCL, India)

**Benchmark Reference**: STMicroelectronics 65nm Standard Cell Library

**Executive Summary**  This analysis identifies a drive-strength gap in the AND and XOR gate families of the SCL 180nm library. By using STMicroelectronics 65nm delay trends as a baseline, this work proposes the addition of X1.5 drive variant to bridge the performance gap found in the low-drive region.

**Analysis Basis & Methodology**  Target Families: 15 variants across AND and XOR logic gates.
Benchmarking: A normalized delay comparison was conducted between the SCL 180nm and STMicroelectronics 65nm libraries.
Focus Area: The analysis focused on drive-granularity needs for marginally critical paths rather than adding new logic functions.

**Key Findings & Evidence**  Performance Disparity: The 180nm normalized delay points consistently stay above the STMicroelectronics 65nm trend in the low-drive region.
Coarse Laddering: The existing jump from X1 to X2 in the SCL library is too coarse compared to the finer granularity found in more advanced nodes like 65nm.

**Recommendations for SCL 180nm Library**  Introduction of X1.5 Drive Strength.
1. Primary Action: Add X1.5 as a primary remap target between X1 and X2.
2. Justification: This is the most defensible intermediate step for both AND and XOR families based on the normalized low-drive comparison.
