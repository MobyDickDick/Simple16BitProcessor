CPU16_Digital_Template

Files:
  - CPU16_TwoPhase_Template.dig   (top-level scaffold)
  - Control16_TwoPhase.dig        (stub module, define Exec/Commit/Phase)
  - CPU16_Regs.dig               (pre-wired: D_FF(16) registers for PC/NPC/IR/A/ADDR; clocks: ExecEn/CommitEn)
  - InstrMem16.dig               (stub module, put a ROM here)

How to use in Digital:
  1) Put all *.dig files into one folder.
  2) Open CPU16_TwoPhase_Template.dig.
  3) Double-click a block to open its subcircuit file and implement its internals.

Notes:
  - The top-level only connects a minimal "fetch" path: PC_out -> InstrMem.ADDR -> IR_in.
  - Most inputs (PC_in/A_in/ADDR_in) are intentionally left unconnected in the scaffold.
