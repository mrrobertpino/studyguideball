# AI Study Guide

A static study guide based on Robert Pino's Lineball and BayesBall teaching tools. It includes Super Summary, The Five Steps, Naive Bayes, Linear Classifier, Machine Learning, Compare Models, and a practice Quiz with automatic answer checking.

## Put it on GitHub Pages

1. Create a GitHub repository, or open the repository you want to use.
2. Upload `index.html` and `.nojekyll` to the repository root and commit the files.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose your branch (usually `main`) and **/ (root)**, then save.
6. GitHub will show the published URL on the Pages settings screen after deployment finishes.

There is no build step, server, API key, or package installation. Hash navigation works on GitHub project pages. To preview locally, open `index.html` in a browser.

The movie posters load from the original Lineball repository and require an internet connection. All lessons, calculations, and quizzes are contained in `index.html`. Student work stays in the current page session and resets on reload; no student data is submitted or collected.

## Teaching notes

- Five steps: Dataset, Train, Test, Inspect, Evaluate.
- Naive Bayes uses 20 original BayesBall messages (seven Personal, seven Promotional, six Spam), the original tokenization and stop words, and add-one smoothing. All counts and probabilities are recalculated for this smaller dataset. Unknown words are ignored; equal scores choose Personal first.
- The Linear Classifier tab preserves the source movie examples and their original weights. Zero is shown as a decision point.
- The Machine Learning tab shows two independent, single training updates: The Godfather pushes weights toward BAD and Cats pushes them toward GOOD. Each starts with the original Lineball weights and updates only weights for present features. The numerical shifts do not change either predicted class after that one update.
- Quiz grading counts unanswered questions as incorrect and gives explanations for every question. Students can change answers and grade again.

Sources: https://github.com/mrrobertpino/lineball and https://github.com/mrrobertpino/sortball4

Movie judgments and message labels are classroom examples, not universal facts.

The Overview includes an ungraded five-question prequiz with targeted page recommendations. The final quiz contains 18 questions, including score calculations and model-failure scenarios. The sticky five-step navigation follows the current scroll position.
