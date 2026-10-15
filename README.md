# AI Study Buddy

An affordable, personalized learning companion for school students (grades 8 to 12).
Built as a project for **IBM SkillsBuild, Masterclass 5: Creating Real Life Projects**.

## The problem
Students get stuck on concepts with nobody to ask after class, private tutoring is expensive, and
classrooms move at one pace. Small learning gaps grow into lost confidence.

## The solution
A patient tutor in your pocket, available 24/7:

- Ask a doubt by **text or a photo** of the question
- Get **step-by-step explanations** that teach the method, in English, Hindi, Marathi, Tamil or Bengali
- **Explain simpler**, **Another example** and **Read aloud** options
- **Quiz me** with 3 multiple-choice questions and instant feedback
- **Progress tracking** (score and recent doubts) saved in the browser
- Menu bar with Ask, Progress and About tabs

## Project documents
| Document | File |
|---|---|
| Lean Canvas | [docs/Lean_Canvas_AI_Study_Buddy.pdf](docs/Lean_Canvas_AI_Study_Buddy.pdf) |
| Concept Note | [docs/Concept_Note_AI_Study_Buddy.pdf](docs/Concept_Note_AI_Study_Buddy.pdf) |
| Presentation | [docs/AI_Study_Buddy_Presentation.pptx](docs/AI_Study_Buddy_Presentation.pptx) |

## Repository structure
```
.
├── index.html      # the prototype (single file: HTML, CSS, JavaScript)
├── docs/           # Lean Canvas, Concept Note, presentation
├── LICENSE
└── README.md
```

## Running the prototype
`index.html` is a single self-contained file with no build step. The page layout, menu, quiz scoring
and progress tracking work in any browser.

**Important:** the AI features (explanations, photo questions, quizzes) use Claude's built-in
page connection (`claude.use("sample")`), so they work only when the page is opened inside Claude.
Opened elsewhere, for example on GitHub Pages, the page shows a message and the AI buttons stay off.

To run the AI features outside Claude, replace the `sample(...)` calls in `index.html` with requests to
your own backend, which should call an AI API and keep the API key on the server. Never put an API key in
front-end code.

## Business model (from the Lean Canvas)
Freemium with a low-cost subscription, school and institution licences, and CSR or NGO sponsorships
for free access for underprivileged students.

## Roadmap
- Pilot with 2 to 3 schools and a few teachers
- Teacher review of content
- More subjects and regional languages
- Backend so the app runs outside Claude
- Weak-topic insights and learning streaks

## Disclaimer
AI explanations can be wrong. Check important answers with a teacher or textbook.
This is a student prototype.

## Author
[Your Name]

## License
MIT, see [LICENSE](LICENSE).
