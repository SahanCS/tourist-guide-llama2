Fine-Tuning LLaMA-2 for a Tourist Guide Assistant
📌 Overview
This project fine-tunes LLaMA-2 to act as a Tourist Guide Assistant for Sri Lanka, providing travel recommendations, city guides, and cultural insights.

🚀 Model Selection
Chosen Model: LLaMA-2
Reason: While GPT-3.5 Turbo is ideal for conversational models and offers better performance, it requires paid fine-tuning. Due to financial constraints, LLaMA-2 is used for this project as an alternative.
📂 Dataset
The dataset (train_data.jsonl and test_data.jsonl) consists of question-answer pairs related to Sri Lankan tourism. Due to resource constraints, we generated a lower number of examples with fewer tokens, which limits the scope of the model. A larger dataset with more tokens would enhance the model’s performance. For future improvements, we recommend increasing the dataset size.


Prompt used for fine-tuning: The model was fine-tuned with the following prompt:

python
Copy
Edit
prompt = "You are a smart and friendly AI-powered tourist guide specializing in Sri Lanka. Your goal is to provide up-to-date, insightful, and engaging information about Sri Lanka's tourist attractions, cultural sites, historical landmarks, local events, and natural wonders. You also offer expert recommendations on local cuisine, must-try Sri Lankan dishes, famous restaurants, street food hotspots, and traditional dining experiences. Additionally, you help travelers find the best accommodations, including luxury hotels, boutique stays, eco-lodges, and budget-friendly options across different cities like Colombo, Kandy, Galle, and Ella. You provide travel tips, safety guidelines, visa regulations, transportation advice, and cultural etiquette to ensure a smooth and enjoyable journey for tourists. Your responses should be warm, detailed, and infused with local insights, making every traveler feel welcome and well-informed. If needed, personalize suggestions based on the traveler's interests, whether they seek adventure, relaxation, history, or culinary delights."
Fine-Tuning Setup:

Temperature: 0.4 (adjusted for conversational tone and consistency).
Number of examples: 10 (kept low due to resource availability, but this can be increased for better performance).
💡 Considerations for Future Improvements
While LLaMA-2 has been used in this project due to its open-source nature, GPT-3.5 Turbo would have been a more suitable choice for the following reasons:

Better Performance for Conversational Models: GPT-3.5 Turbo excels in maintaining a coherent and engaging conversational flow, making it more appropriate for this tourist guide application.
No Architectural Changes Required: GPT-3.5 Turbo offers a robust, ready-to-use conversational framework, meaning no changes to the architecture are necessary for deploying a fully-functional assistant.
Memory Management: LLaMA-2 requires significant memory resources to run locally, while GPT-3.5 Turbo leverages OpenAI’s resources to handle large-scale computations and memory management efficiently.
📂 Project Files
The project includes:

train_data.jsonl: Training data for fine-tuning.
test_data.jsonl: Test data for evaluating the fine-tuned model.
Colab Notebook: For the complete fine-tuning and inference process.
