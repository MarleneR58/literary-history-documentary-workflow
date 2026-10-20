# Literary History Documentary Video Workflow

A customizable browser workflow for making short, historically grounded documentaries about novels, authors, art, ideas, institutions and events. It preserves the original VideoExpress and CloneVoice production process while adapting the story plan to each subject's documented history and creation or publication process.

This personal version is forked from [ai-playbooks/historical-documentary-video-workflow](https://github.com/ai-playbooks/historical-documentary-video-workflow). The original repository remains unchanged.

## What this workflow covers

- Historical setting, creators and participants, motivation, context, changes over time, reception and significance.
- The process that fits the subject: writing, editing, publication, performance, distribution, implementation or construction when construction is actually relevant.
- A photorealistic presenter introduction followed by antique watercolor and ink documentary scenes.
- A narration track, scene-by-scene coverage and timeline assembly in VideoExpress.

For literary subjects, it separates the fictional story from the author's life and the work's publication history. It asks the producer to verify editions and dates, distinguish evidence from illustrative reconstruction, and treat controversy and later consequences with care.

## Requirements

- A browser-capable agent that can follow SYSTEM_PROMPT.md.
- Access to [VideoExpress](https://app.videoexpress.ai/) and [CloneVoice](https://app.clonevoice.ai/) with generation access.
- Sign in when prompted. The workflow is designed for the visible built-in browser.

This repository contains browser automation instructions. It is not a standalone app or an API workflow.

## Use it

1. Load SYSTEM_PROMPT.md as the instructions for your browser automation agent, or ask the agent to read and follow the file.
2. Start the workflow. It asks for:
   - **Idea or script** — required; can be a topic, a story angle or a supplied script.
   - **Presenter** — Daniel Reed by default; describe changes if wanted.
   - **Ratio** — Landscape 16:9 by default; Vertical 9:16 is supported.
   - **Duration** — 60 seconds by default, up to five minutes total, including a presenter intro of at least 20 seconds.
3. Reply with your choices. For example:

    Idea/Script: Explain how The Picture of Dorian Gray was commissioned, published in 1890, revised for the 1891 book edition, and received by Victorian reviewers. Put the scandal in context without claiming the novel alone caused Wilde's later downfall.
    Presenter: Keep the default.
    Ratio: Landscape.
    Duration: 90 seconds.

4. The agent researches the subject, drafts narration and scene prompts, generates the intro and documentary footage, assembles the timeline, saves the project, and opens the export flow. It stops after creating the export and does not download the video.

## Research and visual standards

- Verify factual claims before adding them to narration or prompts. Prefer primary documents and authoritative library or museum records for publication details.
- Do not invent conversations, locations, motives or exact production moments. Label representative staging as illustrative.
- For books, show the manuscript, editing, printing, publication, readership and reviews only as the evidence supports. Keep scenes from a novel's fictional world distinct from real events.
- Specify period clothing, tools, furnishings, editions and settings. Keep objects and people consistent across shots.
- Documentary footage uses antique watercolor and ink unless you choose another style. The presenter intro stays photorealistic.

The example topic in SYSTEM_PROMPT.md uses facts about the magazine publication and later book edition of Wilde's novel as a model. Recheck all details against scholarly or collection sources when adapting it. See the [British Library overview](https://www.britishlibrary.cn/en/works/picture-of-dorian-gray/) and the [Morgan Library catalog record](https://www.themorgan.org/printed-books/130859).

## Audio and timing

The requested duration guides the initial script. The completed narration is then reused unchanged; it is not regenerated or cut to force an exact runtime. It begins after the actual presenter intro. Documentary video is aligned to the full audio clip, and only excess video is trimmed. The final runtime may differ slightly from the initial estimate.

Routine playback QA and unrequested sharing are omitted. Presenter speech stays audible, documentary clip audio is muted beneath narration, and the project is saved before export.

## Customize your workflow

Edit SYSTEM_PROMPT.md in place to change the intake questions, presenter, style, narration voice, research standards, scene format, duration limits or export steps. Keep browser generation and asset handling instructions aligned with the controls visible in VideoExpress and CloneVoice. Use this fork for your changes; the upstream repository is not modified.

## Files

- SYSTEM_PROMPT.md — production instructions for the agent.
- README.md — this guide.
