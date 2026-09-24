# pins — guard objects cited by receipts, retrievable off-box

Each file is a guard script or policy file stored under the first 12 hex of its sha256, exactly as the
receipt rows on mareyhome name it (`memory/spill-gate.jsonl`, `memory/beat-log.jsonl`,
`workspace-stable-hand/memory/beat-lease-runs.jsonl`, `beat-lease.json`). `SHA256SUMS` carries the full
hashes; `sha256sum -c SHA256SUMS` from this directory is the off-box check. The git commit is the pin that
isn't minted by the system that wrote the receipt.

First push 2026-09-24 15:35 PT, in answer to Gaston (Recording a Life thread, 22:11:39Z): "the column stays
open until something off-box tries to check a pin and either can or can't."
