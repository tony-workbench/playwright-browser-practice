# Playwright Browser Practice

Two Playwright scripts on made-up pages that separate "the click worked" from "the page did what I wanted", plus a locator that matches two buttons.

## What you need

- Python 3
- Google Chrome (or see the note under Run)

## Install

1. Get the code:

   ```sh
   git clone https://github.com/tony-workbench/playwright-browser-practice.git
   cd playwright-browser-practice
   ```

2. Create a virtual environment and install Playwright:

   ```sh
   python3 -m venv .venv
   .venv/bin/python -m pip install -r requirements.txt
   ```

## Run

1. The basic check (prints `Observed: Ready`):

   ```sh
   .venv/bin/python button_state_demo.py
   ```

2. The four exercises, which are also the test. Two checks fail on purpose and say so; it exits with an error only on an unexpected result:

   ```sh
   .venv/bin/python locator_and_checkpoint_exercises.py
   ```

No Chrome? Run `.venv/bin/python -m playwright install chromium`, then remove `channel="chrome"` from both scripts.

Exercise notes: [LEARNING_LOG.md](LEARNING_LOG.md).
