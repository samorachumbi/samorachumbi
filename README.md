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
verdict on shipped work, and **29 agent tools** so it can be driven by asking rather than typing. A
fork of [omdsh-dev/dsh-daily-progress](https://github.com/omdsh-dev/dsh-daily-progress), with the
upstream licence retained and the changes documented.

**[dsh-app-launcher](https://github.com/samorachumbi/dsh-app-launcher)** — a draggable **Apps**
pill in the shell: pick an app and its host-rendered page opens in **its own OS window**, so it can be
dragged to a second screen and left there, with a liveness dot per row. It exists because a host-rendered
page has no way in except a URL — and a bookmark that points at nothing looks exactly like a broken plugin.

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

#### Work with me

I take paid work on the DeepSeek Harness. I sell to teams — the ones putting DSH into a real
workflow, where a broken install costs a day and a plugin that ships badly costs trust.

|  | What you get | From |
|---|---|---|
| **Plugin build** | A dual-face plugin — host routes and tools, plus a real UI mounted into the shell. Installed safely, with a rollback, version-pinned to your harness, and 14 days of fixes. | **$500** |
| **Plugin audit** | A written report you can act on: verdict first, `file:line` findings against a pinned commit, the minimum guardrails, and an honest section on what the plugin does well. | **$250** |
| **Profile rescue** | Diagnosis and recovery for a harness throwing `Cannot read properties of undefined (reading 'prepare')` after a plugin install — and an install method that cannot cause it, verified on a scratch profile. | **$150** |

Each of those is work this page already shows: four published plugins and guides, a client half most
authors never ship, and an install procedure I have recovered from a bricked profile **twice**.

**Start here:** open an issue on any repository here — say which of the three you need and what your
harness is running. I'll tell you honestly if it is not a job I should take.

Nairobi, Kenya · USD rates; KSh and M-Pesa for clients in Kenya.
