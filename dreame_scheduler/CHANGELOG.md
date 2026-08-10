# Changelog

## 0.2.3

- Paired integration 0.2.3: tangle-aware recovery — a cable/cord tangle now gets
  one gentle reverse and then a clear "🪢 please free it by hand" alert, instead
  of repeatedly reversing (which just drags the tangle around). No add-on-side
  changes.

## 0.2.2

- Paired integration 0.2.2 fixes a `return_to_base` loop that could fire
  repeatedly while the dock washed the robot's mop pads (a wash cycle reports as
  "cleaning" even though the robot never left the dock). No add-on-side changes.

## 0.2.1

- New **"Honor native per-room settings"** toggle (General) — on by default; the
  scheduler respects the per-room mode / mop / suction you set in the Dreame app
  (so a sweep-only carpet room is never force-mopped).
- Paired integration 0.2.1: honor-native default, plus clearer self-resolving
  stuck alerts — wheel-motor faults ask you to check the wheels, honest "stuck"
  vs "beached" wording, an "✅ all clear" follow-up once it's back on the dock,
  and a new "can't get home" watchdog that spots a robot circling / repositioning
  but not actually making progress back to the dock (manual runs included).

## 0.2.0

Companion release to the Dreame Scheduler **integration 0.2.0**.

**Add-on**
- Clean-by-hand list and one-tap trap-learner **Apply** in the GUI.
- **Send test notification** button, and a warning for rooms scheduled on no days.
- Branding: wordmark banner as the store logo; Roboto bundled locally so the UI
  font loads correctly through ingress.

**Paired integration 0.2.0** adds self-healing recovery (reverse-out unstick,
beaching detection, block-as-a-moment, obstacle-photo alerts, silent-stuck/
stranded watchdogs), a recurring-trap learner, the multi-day scheduling fix,
per-room **"mop every N sweeps"** cadence, and opt-in **door-retry**.

Full notes: https://github.com/botts7/dreame-scheduler/releases/tag/v0.2.0

## 0.1.0

First public release of the Dreame Scheduler add-on — ingress config GUI, a
Report tab (weekly per-room status, coverage thumbnails, obstacles, run
history), ready-to-paste Lovelace cards, and Floor Plan Studio (Labs, opt-in).
