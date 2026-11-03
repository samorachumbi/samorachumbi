### Samora Chumbi

I build **plugins and tooling for the [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness)** —
both halves of a plugin, the storage-backed tools behind them, and the diagnostics that come out of
running them every day.

---

<!-- dsh-portfolio:begin — generated, do not edit by hand -->

#### Plugins

**5 plugins**, all of them installable today.

**[dsh-app-launcher](https://github.com/samorachumbi/dsh-app-launcher)** — A draggable Apps pill for the harness shell: one click opens a host-rendered plugin page in its own OS window, with a liveness dot per app. `MIT`

**[dsh-cost-bubble](https://github.com/samorachumbi/dsh-cost-bubble)** — A draggable $ pill showing the live estimated API cost of the current chat, with the billed token buckets, cache-hit rate and the peak/off-peak rate band. `MIT`

**[dsh-daily-progress-tab](https://github.com/samorachumbi/dsh-daily-progress-tab)** — A daily-progress tab that answers what to work on now: a Pending/Working/Live venture board ranked by money per build-day, a pool of every undone task, per-project backlogs, a feedback loop and sparks — plus a BUILD TIME model: a stated unit for the effort estimate (one build-day = the daily budget in hours), per-task estHours, a measured capacity reading, per-project burn with an honesty caveat, and a revision trail that keeps a deliberately fluid estimate from becoming a rubber stamp. `BSD-3-Clause (upstream, retained)`
  <br>A fork of [omdsh-dev/dsh-daily-progress](https://github.com/omdsh-dev/dsh-daily-progress) at `bedbd28`, with the upstream licence retained.

**[dsh-domain-watch](https://github.com/samorachumbi/dsh-domain-watch)** — Ask the registry instead of a registrar's dashboard: whether a domain is really registered, the registrar of record, days to expiry, transfer lock — and when a vendor panel and the registry disagree, it names the disagreement instead of averaging it. Four agent tools plus a host-rendered board. `MIT`

**[dsh-media-reader](https://github.com/samorachumbi/dsh-media-reader)** — Read local images, audio and video from DeepSeek Harness — including on text-only model routes, where a picture would otherwise be a dead end. media_probe, media_image, media_audio, media_video and media_evidence, a composer drag-and-drop target, and a verification handoff so an unread image is reported instead of guessed. `Proprietary (all rights reserved)`

<!-- dsh-portfolio:end -->

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

Each of those is work this page already shows: five published plugins and guides, a client half most
authors never ship, and an install procedure I have recovered from a bricked profile **twice**.

**Start here:** open an issue on any repository here — say which of the three you need and what your
harness is running. I'll tell you honestly if it is not a job I should take.

Nairobi, Kenya · USD rates; KSh and M-Pesa for clients in Kenya.
