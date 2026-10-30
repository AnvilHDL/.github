<p align="center">
  <a href="https://github.com/AnvilHDL/anvil">
    <img src="https://raw.githubusercontent.com/AnvilHDL/anvil/master/docs/logo/anvil-horizontal.png" alt="AnvilHDL" width="420">
  </a>
</p>

<p align="center">
  <strong>A general purpose language for safer, yet expressive hardware design.</strong>
</p>

<p align="center">
  <a href="https://anvil.kisp-lab.org/"><strong>Try Anvil</strong></a>
  &nbsp; · &nbsp;
  <a href="https://docs.anvil.kisp-lab.org/">Documentation</a>
  &nbsp; · &nbsp;
  <a href="https://dl.acm.org/doi/10.1145/3779212.3790125">Research paper</a>
  &nbsp; · &nbsp;
  <a href="https://github.com/AnvilHDL/pact">Pact</a>
  &nbsp; · &nbsp;
  <a href="https://arxiv.org/abs/2610.26599">Pact paper</a>
  &nbsp; · &nbsp;
  <a href="https://anvilhdl.zulipchat.com/">Community</a>
</p>

---

**Anvil is a general-purpose hardware description language (HDL) that gives designers control over registers and clock-cycle latency.** Its type system ensures that values are used only while valid and that registers are not overwritten while still in use. This property is called **timing safety** and is enforced at compile time.

**[Pact](https://github.com/AnvilHDL/pact) extends Anvil with session types for communication between components.** Each component declares an interface whose type describes its communication behaviour, control flow, and timing. The compiler checks that every process conforms to its declared type and that the types of processes composed together are compatible. Compatible processes exchange messages synchronously without deadlocking. This property is called **communication safety** and is enforced at compile time.

Pact can also check compatibility in an **open setting**, where some components are not yet available. This allows designers to build large systems incrementally.

Anvil and Pact designs compile to synthesizable SystemVerilog.

<table>
  <thead>
    <tr>
      <th align="left">Timing safety</th>
      <th align="left">Communication safety</th>
      <th align="left">RTL expressiveness</th>
      <th align="left">Hardware efficiency</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Anvil's type system enforces <em>timing safety</em> <em>modularly</em>.</td>
      <td>Pact's session types ensure that composed components never deadlock and keep making progress.</td>
      <td>Designers control registers and cycle-level latency.</td>
      <td>Anvil designs add no clock-cycle latency and have minimal overhead in area, power, and frequency. Pact designs also add no clock-cycle latency.</td>
    </tr>
  </tbody>
</table>

## Get started

Run a program in the [online playground](https://anvil.kisp-lab.org/), work through the [tutorial](https://docs.anvil.kisp-lab.org/tutorial/index.html), or [install the compiler](https://docs.anvil.kisp-lab.org/tutorial/installation.html). The [language reference](https://docs.anvil.kisp-lab.org/langref/index.html) covers syntax and semantics.

## Repositories

- **[Anvil compiler](https://github.com/AnvilHDL/anvil)** — The compiler, tests, and example hardware designs.
- **[Language server](https://github.com/AnvilHDL/anvil-lsp)** — Experimental language support and editor extensions for VS Code and Vim/Neovim.
- **[Documentation](https://github.com/AnvilHDL/anvil-docs)** — The source for the documentation site, tutorial, and language reference.
- **[Evaluation experiments](https://github.com/AnvilHDL/AnvilHDL-Experiments)** — Evaluation designs, test harnesses, synthesis reports, and reproduction instructions.
- **[RISCy experiment](https://github.com/AnvilHDL/anvil-RISCy-Experiment)** — A simple pipelined RISC-V processor written in Anvil.
- **[Pact compiler](https://github.com/AnvilHDL/pact)** — Anvil extended with session types and compatibility checking.
- **[Pact language server](https://github.com/AnvilHDL/Pact-LSP)** — Diagnostics for session-type and compatibility errors, completion, hover, and navigation, with VS Code and Vim/Neovim extensions.
- **[Pact experiments](https://github.com/AnvilHDL/Pact-Experiments)** — Pact benchmarks, SystemVerilog references, and the scripts for the POPL 2027 evaluation.
- **[Pact formalization](https://github.com/AnvilHDL/Pact-formalization)** — The Lean 4 mechanization of Pact's type system.

## Publications

1. Aditya Ranjan Jha, Jason Zhijingcheng Yu, Umang Mathur, and Prateek Saxena. 2027. **[A Type System for Communication-Safe Hardware Design](https://arxiv.org/abs/2610.26599)**. *Proceedings of the ACM on Programming Languages* (POPL 2027). Conditionally accepted. arXiv: [2610.26599](https://arxiv.org/abs/2610.26599).

   [BibTeX](https://github.com/AnvilHDL/pact#citing) · [arXiv](https://arxiv.org/abs/2610.26599) · [Artifact](https://doi.org/10.5281/zenodo.23301148)

1. Jason Zhijingcheng Yu, Aditya Ranjan Jha, Umang Mathur, Trevor E. Carlson, and Prateek Saxena. 2026. **[Anvil: A General-Purpose Timing-Safe Hardware Description Language](https://dl.acm.org/doi/10.1145/3779212.3790125)**. In *Proceedings of the 31st ACM International Conference on Architectural Support for Programming Languages and Operating Systems* (ASPLOS ’26). Association for Computing Machinery. DOI: [10.1145/3779212.3790125](https://doi.org/10.1145/3779212.3790125).

   [BibTeX](https://docs.anvil.kisp-lab.org/#anvil-citation) · [Evaluation artefacts](https://github.com/AnvilHDL/AnvilHDL-Experiments)

## Join the discussion

For discussions please join [AnvilHDL Zulip community](https://anvilhdl.zulipchat.com/). Report bugs or propose changes through the [compiler](https://github.com/AnvilHDL/anvil/issues), [Pact compiler](https://github.com/AnvilHDL/pact/issues), [Pact language server](https://github.com/AnvilHDL/Pact-LSP/issues), [language server](https://github.com/AnvilHDL/anvil-lsp/issues), or [documentation](https://github.com/AnvilHDL/anvil-docs/issues) issue trackers. Contributions are welcome.

## Collaboration

For collaborations or queries, please reach out to one of the maintainers:

- [Jason Zhijingcheng Yu](https://corank.info/)
- [Aditya Ranjan Jha](https://arjha.com/)
- [Umang Mathur](https://www.comp.nus.edu.sg/~umathur/)
- [Prateek Saxena](https://www.comp.nus.edu.sg/~prateeks/)
