# From Labs to Bullets

**A daily technical training diary for IT students. It turns hands-on labs into study prompts, training summaries, and resume bullets.**

👉 **Open the app:** https://github.com/Labs-to-Bullets/from-labs-to-bullets/

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

**Days without labs:** students describe what they learned in their own words instead. On lab days, an optional notes box captures anything else from class worth remembering.

## The two study tools

The app writes the prompts and the student pastes them into their own AI tool. The app itself never contacts an AI service.

| Tool | What it does | Best time to use it |
|---|---|---|
| **Listener** | You explain a topic in your own words. The AI grades your explanation on accuracy, completeness, clarity, and use of technical terms, then tells you what you missed. | After class, to check that you really understand. |
| **Examiner** | Quizzes you one question at a time, from basic recall up to exam-style scenarios. It gets harder until you miss, so you know your level. | Before a quiz or exam. |

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

## Your data stays on your laptop

- **No accounts, no sign-in, no server.** Everything you type is saved only in your web browser, on your own laptop.
- **Nobody else can see your entries,** including your instructor and the people who maintain this repository.
- **Use the same browser on the same laptop every day.** Entries saved in Edge won't appear in Chrome, and the reverse.
- **Download a backup every Friday** from **Settings & backup**, and keep it somewhere safe such as OneDrive. If your browser data is cleared, the backup is the only way to get your entries back.
- **New laptop?** Open the app there and choose **Restore from file**.

## Getting started (students)

1. Open the app link above and bookmark it.
2. Enter your training start date and your IT experience level.
3. At the end of each class day, open **Today** and answer the questions.
4. Click **Save & get study prompts**, copy a prompt, and paste it into your AI tool.
5. On Fridays, complete the weekly review and download a backup.

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
- Data is stored in the browser's `localStorage`. Backups are plain JSON files.
- Works in current versions of Microsoft Edge, Google Chrome, Firefox, and Safari, on laptops and phones.
- Supports light and dark mode automatically.
