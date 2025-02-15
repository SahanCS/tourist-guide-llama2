Fine-Tuning LLaMA-2 for a Tourist Guide Assistant
📌 Overview
This project fine-tunes LLaMA-2 to serve as a Tourist Guide Assistant for Sri Lanka, providing travel recommendations, city guides, and cultural insights. The model is trained on curated data to offer engaging and informative responses about Sri Lankan attractions, cuisine, accommodations, and travel tips.

🚀 Model Selection
Chosen Model: LLaMA-2
Reasoning: While GPT-3.5 Turbo is ideal for conversational models and offers better performance, it requires paid fine-tuning. Due to financial constraints, we selected LLaMA-2, which is open-source and provides a viable alternative for this project.
📂 Dataset
The dataset consists of question-answer pairs related to Sri Lankan tourism:

train_data.jsonl – Used for training the model.
test_data.jsonl – Used for evaluating model performance.
⚠️ Resource Constraints: Due to limited resources, we generated fewer training examples with fewer tokens, which restricts the model's learning scope. For better performance, a larger dataset with more tokens is recommended.

📝 Fine-Tuning Prompt
The model was fine-tuned using the following prompt:

python
Copy
Edit
prompt = "You are a smart and friendly AI-powered tourist guide specializing in Sri Lanka. Your goal is to provide up-to-date, insightful, and engaging information about Sri Lanka's tourist attractions, cultural sites, historical landmarks, local events, and natural wonders. You also offer expert recommendations on local cuisine, must-try Sri Lankan dishes, famous restaurants, street food hotspots, and traditional dining experiences. Additionally, you help travelers find the best accommodations, including luxury hotels, boutique stays, eco-lodges, and budget-friendly options across different cities like Colombo, Kandy, Galle, and Ella. You provide travel tips, safety guidelines, visa regulations, transportation advice, and cultural etiquette to ensure a smooth and enjoyable journey for tourists. Your responses should be warm, detailed, and infused with local insights, making every traveler feel welcome and well-informed. If needed, personalize suggestions based on the traveler's interests, whether they seek adventure, relaxation, history, or culinary delights."
⚙️ Fine-Tuning Setup
Temperature: 0.4 (adjusted for conversational tone and consistency).
Number of Training Examples: 10 (limited due to resource availability, but increasing this will improve performance).
💡 Considerations for Future Improvements
While LLaMA-2 is used due to its open-source nature, GPT-3.5 Turbo would have been a more suitable choice for the following reasons:

✅ Better Performance: GPT-3.5 Turbo is highly optimized for conversational AI, making it more suitable for a tourist guide assistant.
✅ No Architectural Changes Needed: GPT-3.5 Turbo comes with built-in conversational optimization, requiring no additional modifications.
✅ Memory Management: LLaMA-2 requires significant local memory, whereas GPT-3.5 Turbo leverages OpenAI's cloud resources, making it more efficient for large-scale computations.
📂 Project Files
This repository includes the following files:

train_data.jsonl – Training dataset for fine-tuning.
test_data.jsonl – Test dataset for model evaluation.
Colab Notebook – Full fine-tuning and inference process (View Notebook).
Fine-Tuned Model – Download the trained model from Google Drive.