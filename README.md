# Medical Dialogue 

## Introduction
Welcome to the Medical Dialogue project! This repository contains a conversational model trained on medical dialogues, capable of generating responses to various prompts related to healthcare. This README file serves as a guide to using the model effectively.

## Getting Started
To use the conversational model, follow the steps below:

1. **Clone the Repository**: Clone this repository to your local machine using Git.
    ```bash
    git clone https://github.com/your-username/medical-dialogue.git
    ```

2. **Install Dependencies**: Ensure you have all the necessary dependencies installed. You may need to install Python and pip if you haven't already. 

3. **Download the Pre-trained Model**: Download the pre-trained model from the provided link and save it to the appropriate directory within the cloned repository.

4. **Run Inference**: Utilize the provided script to interact with the model. 
    
5. **Provide Input**: Input prompts related to medical dialogue when prompted by the script. The model will generate responses based on the provided input.

## Model Configuration
The conversational model is based on the [LLama framework](https://github.com/The-Llama-Team/LLAMA), specifically trained on medical dialogue data. It utilizes a custom architecture optimized for medical text generation.

### Model Parameters
- Context Length: 4096
- Number of CPU Threads: 4
- Number of GPU Layers: 0

### Generation Settings
- Max Tokens: 200
- Stop Tokens 
- Echo Prompt: False
- Top-k Sampling: 1 (Greedy Decoding)

## Contributing
We welcome contributions to enhance the functionality and performance of the conversational model. If you're interested in contributing, please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
We would like to thank the contributors to the LLama framework for providing the foundation for this project.

## Contact
For any questions or feedback, please contact 
