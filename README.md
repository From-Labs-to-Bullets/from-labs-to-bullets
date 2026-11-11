# From Labs to Bullets

**A daily technical training diary for IT students. It turns hands-on labs into study prompts, training summaries, and resume bullets.**

👉 **Open the app:** https://from-labs-to-bullets.github.io/from-labs-to-bullets/

---

## What it does

Over 17 weeks of IT technical training, students complete close to 100 virtual labs and attend lectures and discussions on the same concepts. From Labs to Bullets helps them keep a record of that work and put it to use.

1. **Log each class day (Monday to Thursday).** Answer a few questions about the topics covered, the labs completed, the technologies used, and what each lab accomplished.
2. **Study with AI.** After saving a day, get two ready-to-paste prompts built from your own notes. Use them with any AI tool (Microsoft Copilot, ChatGPT, Claude, Gemini, and others).
3. **Review your week on Fridays.** Reflect on wins, weak spots, and confidence, and get a weekly summary prompt.
4. **Turn your training into career material.** Generate prompts for training summaries, resume bullets, and interview stories from everything you've logged.

## The daily questions

Questions 1 to 5 are required. Questions 6 and 7 are optional.

1. What topics were covered in class today?
2. How many labs did you complete today?

For each lab:

3. What did you build, configure, deploy, or automate in the virtual lab, and what specific technologies or tools did you use to accomplish it?
4. How did the environment or solution function after you completed the lab, and what business or technical objective did your setup achieve? What problem were you trying to solve?
5. What was the scope of the lab environment, including the number of systems, devices, accounts, or automation scripts you configured?

Then:

6. What resources were you given by the instructor that you may want to use later?
7. What was the most interesting or surprising skill, command, technology, or concept you learned today, and why did it stand out to you?

**Scope (question 5):** the app explains why numbers matter for resume bullets and offers examples for each area of the program, including what to write when there's nothing to count.

**Week 9 (Pro-Dev Week):** week 9 is always dedicated to professional development, so the app doesn't track it. There's nothing to log that week, and the app suggests using Summaries & bullets to turn weeks 1 to 8 into resume bullets and interview stories.

**Mock interview days:** mock technical interviews usually happen in week 10 or 11, depending on the cycle. On any class day, students can switch **Type of day** to **Mock interview** to answer three short questions instead: which topics or questions they were asked, which answers felt strong or weak, and what they'll review next. The study prompts then focus on the weak answers. Interview practice, project ideas, and AI discussions are never turned into resume bullets.

**Days without labs:** students describe what they learned in their own words instead. On lab days, an optional notes box captures anything else from class worth remembering.

## The two study tools

The app writes the prompts and the student pastes them into their own AI tool. The app itself never contacts an AI service.

| Tool | Helps you | What it does | Best time to use it |
|---|---|---|---|
| **Listener** | **Understand** | You explain a topic in your own words. The AI grades your explanation on accuracy, completeness, clarity, and use of technical terms, then tells you what you missed. | When a topic is new, to check that you really understand it. |
| **Examiner** | **Remember** | Asks you questions one at a time, answered from memory, from basic recall up to job-style scenarios. It then goes back over the questions you missed and ends with a "Practice next time" list instead of a grade. | To make terms, commands, and steps stick. Also a good warm-up before mock interviews. |

Students are encouraged to try both and use whichever helps them more.

**Refresh (spaced review):** in **Study prompts**, the **Refresh** option builds an Examiner prompt from earlier weeks: up to two days from the last two weeks, two from two to five weeks ago, and two from longer ago. Recalling material again after days or weeks is what keeps it from fading. The mix changes once a day, and students are encouraged to use it once or twice a week.

Every prompt includes the student's notes, their IT experience level, and ground rules telling the AI to:

- stay within the topics the student actually covered,
- use current Microsoft product names,
- say when it isn't sure instead of guessing,
- point the student to Microsoft Learn to check answers.

> **AI can be wrong.** Treat it as a practice partner, not the final word. If an answer doesn't match your lab or class, check Microsoft Learn or ask your instructor.

## Resume bullets

The app builds a prompt that turns logged labs into resume bullets using this format:

**Action + Technology + Purpose**

- **Action:** start with what you did (built, configured, deployed, automated).
- **Technology:** name the specific tools you used.
- **Purpose:** finish with what the setup accomplished.

*Example:* Configured Azure Virtual Networks and Network Security Groups to segment workloads and block unauthorized inbound traffic.

The prompt tells the AI to use only facts from the student's notes, never invent numbers or results, and present the work as hands-on training rather than job experience. Students can save the bullets they like inside the app.

The **Summaries & bullets** tab also builds prompts for:

- a **training summary** of the skills and technologies practiced, and
- **interview stories** in STAR format (Situation, Task, Action, Result).

Each can cover all of training, a single week, a course, or a date range.

## Your data stays on your computer

- **No accounts, no sign-in, no server.** Everything you type is saved in your web browser, on your own computer.
- **Nobody else can see your entries,** including your instructor and the people who maintain this repository.
- **Turn on auto-save.** The last setup step asks students to choose a file, ideally in their **OneDrive** folder. The app then saves the diary to that file every time they type, so clearing the browser's data never erases their work. Auto-save can also be turned on or changed later in **Settings & backup**.
- **Edge asks for permission during the first few visits.** The app shows **Auto-save is paused**; students click **Resume auto-save**, then **Allow**. From the second return visit, Edge also offers **Allow on every visit**. Once students choose it, Edge stops asking.
- **Browser data cleared, or a new computer?** Open the app, choose **I already have a diary file** (or **Open my diary file** in **Settings & backup**), and pick the file. Everything comes back, up to the last thing typed.
- **Use Microsoft Edge on your computer.** Auto-save works in Edge and Chrome on a computer, not in Firefox, Safari, or on phones. Don't use InPrivate windows.
- **Without auto-save, download a backup every Friday** from **Settings & backup**. Students who skip auto-save see a weekly reminder to turn it on and backup reminders.

## Getting started (students)

1. Open the app link above in Microsoft Edge and bookmark it.
2. Enter your training start date and your IT experience level.
3. Turn on auto-save and save your diary file in your OneDrive folder.
4. At the end of each class day, open **Today** and answer the questions.
5. Click **Save & get study prompts**, copy a prompt, and paste it into your AI tool.
6. On Fridays, complete the weekly review.

## For instructors

### Updating the app

The whole app is a single file, `index.html`. To publish a new version:

1. In this repository, click **Add file**, then **Upload files**.
2. Drag in the new `index.html`.
3. Click **Commit changes**.

GitHub Pages updates the live site within a minute or two. Students' saved entries are not affected.

> **Keep the same web address.** Each student's entries are tied to the app's exact URL. If the app moves to a different address, students must download a backup from the old address and restore it at the new one.

### Course list

The **Course or module** list is preloaded with:

- AZ-040: Automating Administration with PowerShell
- GH-900: GitHub Foundations
- Windows Server: Installation, Storage and Compute
- Windows Server: Networking
- Windows Server: Identity
- Linux Administration Fundamentals (Ubuntu)
- AZ-900: Azure Fundamentals
- AI-901: Microsoft Azure AI Fundamentals
- AZ-400: DevOps Solutions
- MD-102: Endpoint Administrator
- AZ-104: Azure Administrator
- SC-300: Identity and Access Administrator

If a course isn't listed, students can choose **+ Add a new course…** at the bottom of the dropdown on the daily log. The course is added to their own list and offered on every day after that. They can also edit or remove courses in **Settings & backup**. This keeps the app useful when the curriculum changes from one cycle to the next.

To change the default list for a new cohort, edit `DEFAULT_COURSES` near the top of the script in `index.html`.

### Lab lists

No lab list is built in, because labs can change from one cohort to the next. Students paste each lab's title from their lab platform. The app remembers the technologies each student enters and suggests them next time.

## Technical details

- A single, self-contained HTML file (HTML, CSS, and JavaScript). There is no build step, and it uses no external libraries.
- Data is stored in the browser's `localStorage`. Backups and the auto-save file are plain JSON files.
- Auto-save uses the browser's File System Access API (Edge and Chrome on a computer). The file's location is remembered in IndexedDB. On startup, the app compares the file with the browser copy and keeps the newer one. Nothing is sent to a server.
- The app asks the browser for persistent storage, so the browser won't remove its data on its own when disk space runs low.
- Designed for Microsoft Edge on Windows. The rest of the app also works in Chrome, Firefox, and Safari, but auto-save is only available in Edge and Chrome.
- Supports light and dark mode automatically.
