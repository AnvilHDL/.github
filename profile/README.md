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
  <a href="https://anvilhdl.zulipchat.com/">Community</a>
</p>

---

**Anvil is a general-purpose hardware description language (HDL) that gives designers control over registers and clock-cycle latency.** Its type system ensures that values are used only while valid and that registers are not overwritten while still in use. This property is called **timing safety** and is enforced at compile time.

Anvil designs compile to synthesizable SystemVerilog.

<table>
  <thead>
    <tr>
      <th align="left">Type system</th>
      <th align="left">RTL expressiveness</th>
      <th align="left">Hardware efficiency</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Anvil's type system enforces <em>timing safety</em> <em>modularly</em>.</td>
      <td>Designers control registers and cycle-level latency.</td>
      <td>Anvil designs add no clock-cycle latency and have minimal overhead in area, power, and frequency.</td>
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

## Publications

1. Jason Zhijingcheng Yu, Aditya Ranjan Jha, Umang Mathur, Trevor E. Carlson, and Prateek Saxena. 2026. **[Anvil: A General-Purpose Timing-Safe Hardware Description Language](https://dl.acm.org/doi/10.1145/3779212.3790125)**. In *Proceedings of the 31st ACM International Conference on Architectural Support for Programming Languages and Operating Systems* (ASPLOS ’26). Association for Computing Machinery. DOI: [10.1145/3779212.3790125](https://doi.org/10.1145/3779212.3790125).

   [BibTeX](https://docs.anvil.kisp-lab.org/#anvil-citation) · [Evaluation artefacts](https://github.com/AnvilHDL/AnvilHDL-Experiments)

## Join the discussion

For discussions please join [AnvilHDL Zulip community](https://anvilhdl.zulipchat.com/). Report bugs or propose changes through the [compiler](https://github.com/AnvilHDL/anvil/issues), [language server](https://github.com/AnvilHDL/anvil-lsp/issues), or [documentation](https://github.com/AnvilHDL/anvil-docs/issues) issue trackers. Contributions are welcome.

## Collaboration

For collaborations or queries, please reach out to one of the maintainers:

- [Jason Zhijingcheng Yu](https://corank.info/)
- [Aditya Ranjan Jha](https://arjha.com/)
- [Umang Mathur](https://www.comp.nus.edu.sg/~umathur/)
- [Prateek Saxena](https://www.comp.nus.edu.sg/~prateeks/)
