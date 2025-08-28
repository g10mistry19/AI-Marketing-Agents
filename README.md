
# AI-Marketing-Agents 🤖✨

A multi-agent system using Crew AI to automate Instagram content strategy and posting.

An autonomous AI agent crew designed to strategize, create, and publish engaging content for Instagram. This project leverages the power of the CrewAI framework to simulate a collaborative marketing team, automating the entire content lifecycle from idea to post.

## 🚀 Overview

This repository contains the code for a multi-agent system that streamlines social media marketing. It consists of two primary agents:

1.  **The Marketing Strategist:** This agent analyzes a given topic or trend and develops a comprehensive content strategy, outlining key themes, post ideas, and target audience engagement points.
2.  **The Instagram Content Creator & Poster:** This agent takes the strategist's plan, crafts compelling captions and relevant hashtags, and then automatically posts the content to a specified Instagram account.

This project is a practical demonstration of how AI agents can collaborate to perform complex, multi-step tasks traditionally handled by a marketing team.

## ✨ Key Features

* **Autonomous Strategy Creation:** Generates marketing plans and content calendars based on simple inputs.
* **Automated Content Generation:** Creates high-quality, relevant captions and hashtag sets.
* **Direct Instagram Publishing:** Seamlessly posts the generated content to Instagram without manual intervention.
* **Collaborative Agent Workflow:** Showcases the power of CrewAI's role-based agent cooperation.
* **Easily Customizable:** Simple to adapt for different topics, brands, or marketing goals.

## 🛠️ Tech Stack

* **Framework:** CrewAI
* **Language:** Python
* **LLMs:** Ollama (Model = Open Herme's 2.5)


## 🤖 CrewAI Framework

CrewAI is designed to facilitate the collaboration of role-playing AI agents. In this example, these agents work together to generate a creative and trendy Instagram post.

---
## ▶️ Running the Script

This example uses **OpenHermes 2.5** through **Ollama** by default, so you will need to download [Ollama](https://ollama.com/) and the [OpenHermes](https://ollama.com/library/openhermes) model.

You can change the model by updating the `MODEL` environment variable in the `.env` file.

1.  **Configure Environment**: Copy the `.env.example` file to a new file named `.env` and set up the environment variables for **Browseless** and **Serper**.
    ```bash
    cp .env.example .env
    ```

2.  **Install Dependencies**: Run `poetry install --no-root` (this project uses `crewAI==0.130.0`).
    ```bash
    poetry install --no-root
    ```

3.  **Execute the Script**: Run `python main.py` and input your idea when prompted.
    ```bash
    python main.py
    ```

---
## ⚙️ Details & Explanation

The script will leverage the CrewAI framework to process your idea and generate a complete Instagram post.

### Key Components:
* `./main.py`: The main script file to execute the crew.
* `./tasks.py`: Contains the prompt definitions for the tasks.
* `./agents.py`: Handles the creation and configuration of the agents.
* `./tools/`: Contains any custom tool classes used by the agents.

---
## 💻 Using Local Models with Ollama

This example is designed to run entirely with both closed and local models, by using tools such as Ollama, for enhanced flexibility and customization. This allows you to utilize your own models, which can be particularly useful for specialized tasks or data privacy concerns.
