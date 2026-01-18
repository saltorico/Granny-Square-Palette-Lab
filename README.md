Granny Square Colour System

This repository contains a single-file interactive HTML tool and its supporting artefacts for designing, previewing, and reasoning about granny square colour systems.

What makes this project different is not just what it produces, but how it came into being: entirely through an extended, iterative design dialogue between a human and AI, with obsessive attention to colour behaviour in real textiles rather than screens.

⸻

What this project is
	•	A palette laboratory for granny squares
	•	Focused on textile realism, not digital colour theory
	•	Built to explore contrast, temperature, material feel, and repetition
	•	Delivered as a self-contained HTML file (no build step, no dependencies)

The tool allows you to:
	•	Define colour palettes using named yarn colours (Toft-inspired)
	•	Assign colours to structural roles (anchor, antagonists, mediator)
	•	Preview individual granny squares
	•	Preview tiled patchwork patterns (with repetition controls)
	•	Iterate rapidly without breaking visual coherence

⸻

How we arrived here (the short version)

This project started with a simple desire:

“Combine Toft yarn colours in ways that are surprising, high-contrast, and not common.”

From there, the conversation unfolded into several deep explorations:

1. Colour as material, not RGB

Early on, we rejected screen-first thinking.
Every colour decision was evaluated as if it were:
	•	yarn
	•	fibre
	•	dyed material under imperfect light

That led to hundreds of micro-adjustments:
	•	removing brown from greys
	•	adding black without darkening
	•	shifting yellow via green, not red
	•	reintroducing blue without going neon

Each colour was tuned until it behaved correctly next to others, not in isolation.

The result is a carefully curated TOFT_HEX table where every value has intent.

⸻

2. Roles instead of colours

Rather than treating colours as interchangeable swatches, we introduced roles:
	•	Anchor – structural calm, visual gravity
	•	Antagonist (cold) – tension via cool contrast
	•	Antagonist (hot) – tension via warmth
	•	Mediator / Instigator – the colour that makes the others speak

This allowed palettes to be:
	•	rotated
	•	inverted
	•	reused

…without falling apart.

⸻

3. From palettes to systems

The work quickly moved beyond single palettes into palette sets:
	•	“Gutsy Toft” (bold, confrontational combinations)
	•	“Maikel’s Scarf” (observed, not designed; inspired by a real scarf)
	•	Future themed sets (cities, films, moods, brands)

To support this, we designed:
	•	a JSON schema for palette sets
	•	import/export functionality
	•	the ability to load arbitrary new sets without touching the HTML

⸻

4. Pattern logic and repetition

Attention then shifted to how colours repeat:
	•	ensuring no identical colours touch
	•	designing a stable 4×4 base pattern (α β γ δ cycling)
	•	enabling repetition (NxM blocks) without visual chaos

Even the direction of shifts (left-rotating rows) was debated and refined to satisfy both visual logic and OCD-level pattern recognition.

⸻

5. Tooling details that matter

A lot of care went into things that seem small, but aren’t:
	•	removing 1px white seams between tiles
	•	eliminating decorative artefacts that interfered with colour reading
	•	making dropdowns searchable by typing
	•	preserving palette order exactly as defined (never auto-sorted)
	•	ensuring previews reflect the current palette, not stale state

These decisions are what make the tool feel calm, trustworthy, and usable for long sessions.

⸻

What’s in this repository
	•	palettes and granny squares.html
	•	the complete interactive tool
	•	open it directly in a browser
	•	JSON palette definitions
	•	human-readable
	•	extensible
	•	designed for sharing and remixing
	•	Documentation (this README + canvas exports)

⸻

Philosophy

This project follows a few strong principles:
	•	Design is discovered, not invented
	•	Colour lives in relationships
	•	Subtlety beats cleverness
	•	Repetition should feel inevitable, not mechanical

If a colour only works alone, it’s wrong.
If a pattern needs explanation, it’s not finished.

⸻

How to use this
	1.	Open the HTML file locally or via GitHub Pages / Netlify
	2.	Select a palette set
	3.	Browse palettes with prev/next or dropdown
	4.	Adjust repetition
	5.	Export previews or palette JSON

No installation. No build. No framework.

⸻

Status

This is a living artefact.
Colours may still be tuned.
New palette sets will be added.
The core philosophy, however, is stable.

⸻

Acknowledgement

This project is the result of sustained, thoughtful collaboration between a human designer and AI — not as a generator of answers, but as a partner in seeing, correcting, and refining.

If you use or adapt this work, do so with the same care it was built with.
