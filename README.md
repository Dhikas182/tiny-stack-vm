# Tiny Stack VM

[![make.fun · tiny-stack-vm-01-run-20261122](https://make.fun/badge/tiny-stack-vm-01-run-20261122.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)
[![rank](https://make.fun/badge/tiny-stack-vm-01-run-20261122/Dhikas182/tiny-stack-vm/rank.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)
[![reward](https://make.fun/badge/tiny-stack-vm-01-run-20261122/Dhikas182/tiny-stack-vm/reward.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)

A make.fun entry for
[tiny-stack-vm-01-run-20261122](https://make.fun/bounty/tiny-stack-vm-01-run-20261122):
a faithful interpreter of make.fun's tiny stack ISA v1, answering
exactly as the reference VM (`program/generator/subject/vm.mjs`)
does — all 36 opcodes, all 10 traps with their own exit codes, the
step and output limits, wrapping `Math.imul`, `-2147483648 / -1`,
unsigned DIVU/MODU/LTU, 5-bit shifts, PUSH8 sign extension, EXIT's
low byte.

`main.ts` (Node 22, stdlib only) reads `/input/<id>/program.bin` +
`input.bin` and writes `/output/<id>/stdout.bin` and `exit.txt`.

Verification (this machine, Node 24.22.1): practice set **40/40**
instances identical to the kit reference, two runs byte-identical,
whole set in well under 1 s (limit 60 s).

Files: `main.ts` — the interpreter; `LICENSE` — MIT.
