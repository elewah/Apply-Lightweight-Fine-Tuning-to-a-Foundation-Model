# 📘 Project1-Apply-Lightweight-Fine-Tuning-to-a-Foundation-Mode

Lightweight fine-tuning is one of the most important techniques for adapting foundation models, as it enables customization with minimal computational resources.

In this project, we demonstrate how to apply **parameter-efficient fine-tuning (PEFT)** using the [Hugging Face `peft`](https://github.com/huggingface/peft) library.

---

## 🚀 Project Summary

This project brings together all the essential components of a PyTorch + Hugging Face training and inference pipeline:

- ✅ Load and evaluate a pre-trained model.
- 🎯 Perform parameter-efficient fine-tuning using the `peft` library.
- 🔍 Run inference using the fine-tuned model and compare it with the original model.

---

## 🛠️ Technologies Used

- [PyTorch](https://pytorch.org/)
- [Hugging Face Transformers](https://github.com/huggingface/transformers)
- [Hugging Face PEFT](https://github.com/huggingface/peft)

---
## 📂 Repository Content

This repository contains the following Jupyter notebooks:

1. **`train_base_model_with_probing.ipynb`**  
    Train a base model using probing techniques to evaluate its performance on specific tasks.

2. **`train_base_model_with_probing_and_peft.ipynb`**  
    Fine-tune the base model using both probing and parameter-efficient fine-tuning (PEFT) to achieve better task-specific performance.

3. **`load_and_infer_from_huggingface_hub.ipynb`**  
    Load pre-trained models from the Hugging Face Hub and perform inference to compare the results of the base and fine-tuned models.

Each notebook is designed to be modular and easy to follow, enabling you to experiment with lightweight fine-tuning techniques effectively.

Feel free to open issues or contribute to this repo if you're interested in exploring lightweight model adaptation!

## ⚙️ Setup Instructions

You can run this project locally or in a GitHub Codespace using the provided development container configuration.

### Running Locally

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/elewah/Apply-Lightweight-Fine-Tuning-to-a-Foundation-Model.git
    cd Project1-Apply-Lightweight-Fine-Tuning-to-a-Foundation-Model
    ```

2. **Install Docker**:  
    Ensure you have [Docker](https://www.docker.com/) installed and running on your machine.

3. **Open in VS Code**:  
    Install the [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension in Visual Studio Code.

4. **Reopen in Container**:  
    Open the project in VS Code and select **"Reopen in Container"** from the Command Palette (`Ctrl+Shift+P`).

5. **Install Dependencies**:  
    Once the container is built, all dependencies will be installed automatically as specified in the `devcontainer.json` file.

### Running in GitHub Codespace

1. **Create a Codespace**:  
    Click the **Code** button on the repository page and select **"Create Codespace on main"**.

2. **Wait for Setup**:  
    The Codespace will automatically build the development container and install all dependencies.

3. **Start Working**:  
    Once the setup is complete, you can start running the notebooks or scripts directly in the Codespace.

    > **Hint**: If you are not using a GPU, make sure to comment out the following line in the `devcontainer.json` file to avoid unnecessary configuration errors:
    > ```json
    > "runArgs": ["--gpus", "all"],
    > ```
Both methods provide a consistent development environment with all required tools and dependencies pre-configured.
