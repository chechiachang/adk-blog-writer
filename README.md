### Initialize Blog Writer from ADK Samples

https://github.com/google/adk-samples/tree/main/python/agents/blog-writer

```
git clone https://github.com/google/adk-samples.git

cp -r adk-samples/python/agents/blog-writer/* .
```

### Set up a .env file with your Google API key

```
GOOGLE_API_KEY=
GOOGLE_GENAI_USE_VERTEXAI=False
```

### Running the Agent and Tests

To run any scripts or tests within the project's virtual environment, use `uv run`:

**Run the main agent (interactive playground):**

```bash
uv run adk web
```

**Run the main agent (command-line interface):**

```bash
uv run adk run blogger_agent
```

**Run the integration test:**

```bash
uv run python -m tests.test_agent
```

**Run the evaluation (smoke test):**

```bash
uv run pytest eval/test_eval.py
```

## Example Conversation

**User:** I want to write a blog post about the new Google Gemini 2.5 Flash Preview model, also known as Nanobanana.

**Agent:** I can do that. Here is a blog post outline for an article about the Google Gemini 2.5 Flash Preview model.

---

## Blog Post Outline: Introducing Gemini 2.5 Flash: Google's Newest, Fastest AI Model

### I. Title
Gemini 2.5 Flash: The Speed and Efficiency of Nanobanana

### II. Introduction
*   **Hook:** Announcing Google's latest AI model, Gemini 2.5 Flash, nicknamed Nanobanana.
*   **Context:** Explain that this new model is designed for speed and efficiency, making it ideal for on-device applications.
*   **Thesis Statement:** This post will explore the key features of Gemini 2.5 Flash, its capabilities, and how it compares to other models in the Gemini family.

### III. Main Body

#### A. What is Gemini 2.5 Flash?
*   **Lightweight and Cost-Effective:** Describe how Gemini 2.5 Flash is a smaller, more efficient model compared to its predecessors.
*   **Multimodal Capabilities:** Explain that it can process text, audio, images, and video.
*   **1-Million Token Context Window:** Discuss the large context window and its implications for processing large amounts of information.
*   **'Thinking' Capability:** Detail the new feature that provides transparency into the model's reasoning process.

#### B. Key Features and Enhancements
*   **Speed and Efficiency:** Emphasize the model's performance on low-power devices.
*   **Controlled Generation, Function Calling, and Search:** Discuss the model's advanced functionalities.
*   **Specialized Versions:** Mention the specialized versions for live API, image generation, and text-to-speech.

#### C. How to Get Access
*   **Availability:** Explain that the model is available through the Gemini API, Google AI Studio, and Vertex AI.

### IV. Conclusion
*   **Summary:** Recap the key features and benefits of Gemini 2.5 Flash.
*   **Call to Action:** Encourage readers to explore the new model and its capabilities.

---

**User:** looks good, write it

**Agent:** You have two options for including visual content in your blog post...
