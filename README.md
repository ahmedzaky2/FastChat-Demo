# 🚀 Deploy FastChat on Google Colab

## 📌 1. Introduction
[FastChat](https://github.com/lm-sys/FastChat) is an open-source framework for serving and interacting with **chat-based large language models (LLMs)**.  
It provides:
- A **controller** to manage connected model workers  
- **Model workers** that load and serve Hugging Face models  
- A **Gradio Web UI** for chatting with models through a web interface  
- An **OpenAI-compatible API server** for programmatic access, similar to the official OpenAI API  

---

## 📌 2. Running on Google Colab
This project demonstrates how to set up and run **FastChat** in a Google Colab notebook.  
Using Colab allows you to quickly test small or medium-sized models without needing your own GPU server.  
In this example, we use **`flan-t5-small`** (a lightweight model) to keep things simple and efficient.

---

## 📌 3. Components & Steps

To run FastChat successfully, four main components need to be started in order:

1. **Controller**  
   - Manages the distributed system  
   - Keeps track of available workers  

2. **Model Worker**  
   - Loads the language model (e.g., flan-t5-small)  
   - Connects to the controller to serve inference requests  

3. **Gradio Web UI**  
   - Provides a user-friendly chat interface in the browser  
   - Generates a temporary public `.gradio.live` link when running in Colab  

4. **OpenAI-Compatible API Server**  
   - Exposes an API endpoint similar to OpenAI’s ChatCompletion API  
   - Allows you to send programmatic requests from Python or other clients  

---

✅ After starting these components, you can either:  
- Use the **Gradio Web UI** (via the generated link) for chatting, or  
- Use the **OpenAI API endpoint** to integrate FastChat into your applications.


