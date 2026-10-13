MCQ Practice Quiz — static website

FILES
- index.html: quiz interface and logic
- questions.json: all 500 questions extracted from the workbook's "Improved MCQs" sheet

FEATURES
- Five sets: Q001–Q100, Q101–Q200, Q201–Q300, Q301–Q400, Q401–Q500
- Questions shuffled every attempt while preserving original IDs
- Optional shuffled answer options
- Records selected answers during the attempt
- Optional timer (30/45/60 minutes or custom)
- Automatic submission when the timer reaches zero
- Results, correct/incorrect/unanswered counts, score, answer key and explanations
- Uses the workbook's score and negative-score columns

RUN LOCALLY
Because browsers may block fetching a JSON file directly from file://, run a local static server from this folder:
  python -m http.server 8000
Then open:
  http://localhost:8000

DEPLOY
Upload both index.html and questions.json to the same folder on any static hosting service (GitHub Pages, Netlify, Vercel, etc.). No backend is required.

NOTE
The website uses the "Improved MCQs" worksheet. The answers are checked locally in the browser; responses are not sent to a server.
