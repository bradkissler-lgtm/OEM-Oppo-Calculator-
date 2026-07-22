# The NO CAPTIVE Cost Calculator

An interactive calculator for Vanguard Captive Management (VCM). Estimates how much an OEM is losing annually by not running a captive or hybrid captive financing program, broken into four value levers:

- **Finance income** — interest-rate spread retained vs. given to a third-party lender
- **Lost sales** — deals that fall through due to financing friction
- **Retention** — repeat purchases lost at trade-in, valued across a customer's next few replacement cycles (multi-year CLV, discounted)
- **Brand impact** — cost of a financing experience bad enough to cost the next sale

Single self-contained file (`index.html`) — no build step, no external dependencies, no backend required to run.

## Hosting via GitHub Pages

Once this repo is pushed to GitHub:

1. Go to the repo's **Settings → Pages**
2. Under "Build and deployment," set **Source** to "Deploy from a branch"
3. Set **Branch** to `main` and folder to `/ (root)`
4. Save — GitHub will publish at `https://<your-username>.github.io/vcm-no-captive-calculator/`

That URL can be embedded on the VCM website via an iframe (see the Squarespace Embed block instructions given separately), or linked to directly.

## Before this goes live to real prospects

- [ ] Wire the secondary lead-capture form (see `TODO(dev)` comment near the bottom of `index.html`) to a real CRM/form endpoint — it currently doesn't submit anywhere
- [ ] Point the "Talk to VCM About Your Captive Options" button to a real contact/scheduling destination — it's currently a placeholder `href="#"`
- [ ] Confirm the brand colors/logo mark against VCM's actual brand guidelines (colors were pulled from the logo directly; the header mark is a CSS approximation, not the real logo file)

## Assumptions

All industry-benchmark assumptions (average unit price, gross margin, financing penetration, replacement cycle, etc.) are visible and editable in the "Refine the assumptions" panel on the calculator itself, and explained in the "How we calculated this" section under the results. These are directional planning estimates, not guarantees.
