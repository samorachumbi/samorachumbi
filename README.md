### Samora Chumbi

I build **plugins and tooling for the [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness)** —
both halves of a plugin, the storage-backed tools behind them, and the diagnostics that come out of
running them every day.

---

#### Plugins

**[dsh-cost-bubble](https://github.com/samorachumbi/dsh-cost-bubble)** — a draggable pill showing the
**live estimated cost of the current chat**, read from provider-reported token usage rather than a
`chars / 4` guess. A host half that registers its own route, a client half that mounts into the shell
overlay. Covers the billed buckets, cache-hit rate, and the peak/off-peak rate band.

**[dsh-daily-progress-tab](https://github.com/samorachumbi/dsh-daily-progress-tab)** — a planner in its
own browser tab. A venture board ranked by *money per day of build effort*, a pool of every undone task
across all days so you can pick what to work on, per-project backlogs, a feedback loop that forces a
verdict on shipped work, and **28 agent tools** so it can be driven by asking rather than typing. A
fork of [omdsh-dev/dsh-daily-progress](https://github.com/omdsh-dev/dsh-daily-progress), with the
upstream licence retained and the changes documented.

#### Writing & diagnostics

**[dsh-plugin-install-guide](https://github.com/samorachumbi/dsh-plugin-install-guide)** — why
`dsh plugin add` can leave a profile with a **split `Symbol`** and kill *every* tool call, the
ten-second check that confirms it, and the install method that cannot cause it. Includes a
`diagnose.sh` that also explains why the common "count the copies" check over-reports.

---

#### What I work on

- **Both halves of a plugin** — a host half that registers routes and tools against the real service
  names, and a client half that mounts into the shell. I have hit, and documented, most of the ways
  that goes wrong.
- **Storage-backed agent tools** — versioned records with no required migration, summaries derived on
  read instead of stored, and tool schemas that make the wrong call impossible rather than unlikely.
- **Verification** — live probes against a real harness instead of mocks, rendered pixels instead of
  "it looks fine", and a written bug census so a trap that bit once does not bite twice.

---

Nairobi, Kenya · samorachumbi@gmail.com
