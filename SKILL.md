---
name: html-courseware
description: 按最终确认的浅色画布风格制作或修改可在浏览器演示的 HTML 课程课件：封面回弹与打字机动效、切页淡入、逐页脚本与同案递进，提供目录、翻页和复制交互。
---

# Build a slide courseware in the confirmed light style

Build a standalone HTML slide deck that matches the confirmed light canvas style, motion, and teaching structure of the reference deck, then verify it before delivery.

## Use the confirmed style

- Build one self contained `index.html` with no external references so it opens offline and projects without network.

- Use a 1920 by 1080 stage that scales to fit the window, with a 300px sidebar, a footer row for navigation, and one slide visible at a time.

- Use the light canvas: page background `#fafafa`, sidebar `#f5f5f5`, white cards with a 1px `#e8e8e8` border and 18px radius, and a near black prompt card `#111` with white text.

- Use black capsules `#111` with white text for the current nav item, copy buttons, and status pills, and use green `#22c55e` only for newly added lines and red `#e5484d` only for practice labels.

- Set the cover title to 120px, weight 900, and line height 1.13, section titles to 56px and weight 900, body text to 30px with line height 1.75, and small gray labels to 20px with 4px letter spacing.

- Give slides 120px top padding, 110px side padding, and 80px bottom padding, and cap single column text at 980px while letting titles, panels, tables, and flows use the full width.

- Put a large pale ghost number on chapter pages, show the current chapter name at the top right, and show a live coordinate readout at the bottom right.

## Build the motion

- Animate the cover title lines with a rise that slightly overshoots, staggered by about 140ms, and play the cover entrance only once by clearing the animation when it ends so returning to the cover does not replay it.

- Type the cover lead with a typewriter loop that types at about 75ms per character, holds about 2300ms, deletes at about 35ms per character, pauses about 1200ms, and shows a blinking cursor with a 1.1 second cycle.

- Change slides with a pure opacity cross fade of about 0.3 seconds and no vertical movement.

- Add a light gray rounded hover background on nav items, a light gray hover background on footer buttons, and a slightly lighter hover background on copy buttons.

- Update the bottom readout live from mouse movement with a 1.08 multiplier, show a real frame rate, and keep the angle at 0.0 degrees unless the design actually has a tilted background.

- Respect reduced motion by showing the full lead text statically and disabling animations.

## Structure the teaching

- Organize the deck in four parts that move from why the skill matters, to the everyday technique, to the reusable rule, to the tool that lets the model act.

- Give each page one core conclusion, show the difference before the method, and layer the same case across pages instead of switching cases.

- When demonstrating a technique step by step, start from a weak version, add one principle per page, color only the newly added words green, and state the green legend on the first page of the sequence.

- Keep each step strictly cumulative so no earlier line silently disappears, and write one short line under each step that says what changed and why it matters.

- Present weak versus strong versions side by side with identical card styling so only the content differs, and add a copy button to every prompt the learner should reuse.

- Show a copy button success message only after the clipboard write succeeds, and fall back to asking for manual selection when it fails.

- Merge an upper and lower page into one scrollable page instead of splitting content, and keep one copy button for the merged whole.

- End a technique chapter with a practice page that names the task, the constraints, the finish standard, the suggested minutes, and the page to check against.

## Keep the content rules

- Never label the deck as a teaching simulation and never mark example data as non real, since the user finds and runs the data themselves.

- Write the uncertain data convention as one word everywhere, and use the word the reusable rule uses so learners never face two conventions.

- Never invent a number, a result, or a product behavior, and soften any product claim into an analogy when the exact mechanism is unconfirmed.

- Make the blank template use exactly the same section headings as the worked example so a learner can copy the template and match the example.

- Keep the five principle mnemonic in principle order and reuse the same five words in the practice check and in the summary.

- Write a reusable rule with the same eight sections in the same order: Profile, Role, Goals, Constraints, Skills, Workflow, OutputFormat, Examples, and Initialization.

- List paradigm frameworks in one table, recommend the three most handy ones for daily work, and tell learners that choosing a framework, filling it, and testing the output is enough.

## Verify before delivery

- Count the slides from the section elements, confirm the footer progress maximum matches that count, and confirm every copy button target exists.

- Parse the file for tag balance, confirm no split page markers remain, confirm no old element ids remain, and confirm the title appears in the browser title, the sidebar brand, and the cover kicker.

- Read every page as the teacher would teach it and fix any heading that lost its meaning, any summary that drops a principle, any section that promises a part the format omits, and any route line that claims a practice the deck does not contain.

- Run keyboard navigation through arrows, PageUp, PageDown, Space, Home, and End, and confirm keys do nothing inside inputs, text areas, selects, buttons, and editable regions.

- State plainly when verification was structural only, since the live browser cannot reach a local server, and ask the user to flip through long pages before projecting.

## Deliver

- Deliver the single `index.html` and a ZIP of its folder in the same message, and keep discussion, reasoning, and quality self assessment out of the deck itself.

- Read the canonical example at `assets/zhaotian-prompt-courseware.html` when a new deck needs to match this style exactly.

## Available connectors

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Alternatives for better results

- Ask the user when they want a different visual style instead of assuming the light canvas fits every topic.

- Split a deck into two decks when one topic needs more than about 35 pages, since a longer deck hurts live teaching more than it helps.
