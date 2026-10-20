# Setting Up Study Buddy

Study Buddy is a set of instructions ([TUTOR.md](TUTOR.md)) that turns a regular AI chatbot into a patient tutor for this study plan. These steps are for whoever sets it up. Once it is set up, the learner just opens the chat and starts talking.

## Easiest: just share the link (no setup)

The learner can open a chatbot that can browse the web and send:

> https://github.com/badtyprr/intro2ai

The README contains a note for AI assistants that points to [TUTOR.md](TUTOR.md), so a chatbot that reads the page should become Study Buddy and greet her on its own.

This depends on the chatbot. It needs web access turned on, and some chatbots treat instructions found on a web page cautiously and may ask what she wants instead. Test it once with the chatbot she will use. If it does not take, use one of the setups below, which work reliably and only need to be done once.

## Reliable: a one-time setup

Pick the chatbot she will use. Each setup takes about 10 minutes.

## Claude (claude.ai) using a Project

1. Go to claude.ai, sign in, and create a new **Project** named "AI Study Plan."
2. In the project's **instructions** field, paste the full contents of [TUTOR.md](TUTOR.md).
3. In the project's **knowledge** area, upload the study plan files: `README.md`, everything in the `weeks/` folder, `concerns-and-safety.md`, `practice-prompts.md`, `glossary.md`, and `progress-checklist.md`.
4. Start a new chat inside the project and type "Hi." Study Buddy should greet her.

## ChatGPT using a custom GPT

1. Go to chatgpt.com, open **GPTs**, and choose **Create**.
2. Open the **Configure** tab. Name it "Study Buddy."
3. Paste the full contents of [TUTOR.md](TUTOR.md) into **Instructions**.
4. Under **Knowledge**, upload the same study plan files listed above.
5. Save it as **Only me** (private), then open it and type "Hi."

## Gemini using a Gem

1. Go to gemini.google.com and open **Gems**, then create a new Gem.
2. Name it "Study Buddy" and paste the full contents of [TUTOR.md](TUTOR.md) into the instructions.
3. Add the study plan files as knowledge if the option is available.
4. Save it, open it, and type "Hi."

## Coding assistants that read this repository

If this repository is opened in Claude Code or another assistant that reads repository instruction files, it will pick up Study Buddy automatically through `CLAUDE.md` and `AGENTS.md` at the top of the repository. This is mainly useful for testing changes to the tutor.

## Quick option, no setup

Open any chatbot, paste the contents of [TUTOR.md](TUTOR.md) as the first message, and add: "Please act as described above. I am starting the study plan." This works for one conversation, but she will need to paste it again next time, so one of the setups above is better.

## Before handing it over

- Turn off the setting that lets her conversations be used for training, if she would prefer that (see Week 3, Step 1).
- Try a few test messages yourself, such as "I'm scared of AI," "Can you just do this for me?" and "I want to stop." Check that the replies are warm, honest, and do not push.
- Changes to the instructions should be made in [TUTOR.md](TUTOR.md) and then copied into the chatbot again.

---

[Back to the plan](../README.md)
