# Provenance

1. The pipeline downloads the official filtered XLSX export beginning at
   `2015-01` from the Bank of Lithuania statistics table.
2. It verifies the workbook source, unit and update timestamp.
3. It selects column G, whose permanent source code is
   `PNS.M.A2V.A.C.A.U2.250.200.N.LT.PC___.E.SR`.
4. Publication requires at least 120 observations, an uninterrupted monthly
   sequence, numeric values between 0 and 30 percent, and a first period of
   `2015-01`.
5. The raw XLSX, resolved URL, retrieval time and SHA-256 are retained.

Release `v2026.05` contains 137 observations through 2026-05. Its source
workbook reports an update timestamp of `2026-06-29 15:00:00`.

Pipeline implementation:
https://bustoduomenys.lt/api/v1/mortgage-rates.json

Primary source:
https://www.lb.lt/lt/paskolu-palukanu-normos
