# Setting Up Study Buddy

Study Buddy is a set of instructions ([TUTOR.md](TUTOR.md)) that turns an AI chatbot into a patient tutor for this study plan. It also saves the learner's progress back to this repository after each finished lesson chunk (see "Saving her progress" in TUTOR.md).

These steps are for whoever sets it up. Do the setup on the learner's own device, signed in to her own accounts. Once it is done, she just opens the chat and starts talking.

## What Study Buddy needs

This repository is private, so the chatbot needs two things through the learner's GitHub account (she must be a collaborator on the repository):

1. **Read access**, to see the lessons and her saved progress.
2. **Write access**, to save her progress. Without it, Study Buddy still teaches, but nothing is saved between sessions.

Test both before handing it over (see the last section).

## Option A (most reliable): Claude Code, connected to this repository

Claude Code runs with a real copy of the repository, so it can read lessons and save progress with no extra steps. It loads Study Buddy automatically from `CLAUDE.md`.

1. Sign in to Claude with the learner's account.
2. Connect her GitHub account and open a Claude Code session on `badtyprr/intro2ai` (from the Claude app or claude.ai/code).
3. Type "Hi." Study Buddy should greet her, read her journal, and pick up where she left off.

For each new study session, she opens a new session on the same repository.

## Option B: Claude chat with a GitHub connection

1. Sign in to claude.ai with the learner's account and connect GitHub with her GitHub account under connectors.
2. Create a **Project** named "AI Study Plan" and paste the full contents of [TUTOR.md](TUTOR.md) into the project instructions.
3. Start a chat in the project and type "Hi."

Whether progress saving works here depends on whether the GitHub connection can edit files in the repository. Check with the test below. If it can only read, Study Buddy will teach but not save.

## Option C: Other chatbots

ChatGPT custom GPTs and Gemini Gems can hold the instructions from [TUTOR.md](TUTOR.md), but they usually cannot read a private repository or save to it. If she uses one of these, upload the lesson files as knowledge, and expect no automatic progress saving.

## Before handing it over

1. **Test reading:** type "Hi." Study Buddy should greet her and mention where she left off, or offer to start at Week 1.
2. **Test saving:** go through a tiny step (for example, say you wrote down two worries for Week 1), then say "I'm done for today." Check on GitHub that `progress/journal.md` and `progress/notes/week-01.md` were updated. Then delete that test entry so she starts clean.
3. **Test the tone:** try "I'm scared of AI," "Can you just do this for me?" and "I want to stop." Replies should be warm, honest, short, and never pushy.
4. **Privacy settings:** turn off the setting that lets her conversations be used for training, if she would prefer that (see Week 3, Step 1).

Changes to the tutor's behavior go in [TUTOR.md](TUTOR.md). Option A picks them up automatically; for Option B or C, paste the updated text into the chatbot again.

---

[Back to the plan](../README.md)
