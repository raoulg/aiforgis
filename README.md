# Installation

You dont need to install the dependencies locally; at the top of the notebooks, there is a "open with colab" button that opens the notebooks in google colab.

Especially for the transfer learning, make sure to select the dropdown menu next to "Connect" or "Verbinding Maken". Select "Change runtime type" or "Runtime type wijzigen" and select the GPU (eg T4 GPU).

You can now run all cells with "Runtime" -> "Run all" or "Runtime" -> "Alles uitvoeren".

If you want to run the notebooks locally, either run

```bash
python -m venv .venv
pip install .
```

Or if you want to speed up installation with a factor 10x-100x, [install uv](https://docs.astral.sh/uv/getting-started/installation/) and run

```bash
uv sync
```

# Exercise

Use a modern model (eg Claude 3.7 Sonnet at claude.ai or Gemini 2.5 Pro at gemini.google.com). As a prompt, use something along these lines:

>"I want to explore the possibilities for using AI in my work context. Please dont to give suggestions immediately, but instead start with asking me questions to learn more about my context. Gather enough information about my problems, and ask follow up questions if things are unclear. Only after you have asked enough questions and follow up questions, and gathered enough information, give me suggestions on how to use AI.Consider strategies like Neural Networks, Image Recognition with CNNs and transfer learning, modified versions of the AlphaGo algorithm (first identify what in my situation would be similar to feature planes, what the action space is, what a good reward function could be and how to implement MCTS) and for optimization problems consider swarm intelligence like GWO, ABC, ACO etc.After you have gathered enough information about my context, give me two suggestions that are obvious things to try, and two other suggestions that might be more experimental or out of the box but with high potential. In your suggestions, be certain to include both an intuitive description that is understandable for someone unfamiliar what AI and a more formal description that can actually be used by someone skilled in building AI algorithms.
