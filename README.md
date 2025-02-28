# **Fine-Tuning LLaMA-2 for a Tourist Guide Assistant**  

## 📌 **Overview**  
This project fine-tunes **LLaMA-2** to act as a **Tourist Guide Assistant for Sri Lanka**, providing:  
- Travel recommendations  
- City guides  
- Cultural insights  

## 🚀 **Model Selection**  
- **Chosen Model:** LLaMA-2  
- **Reason:** While **GPT-3.5 Turbo** is better for conversational models, it requires **paid fine-tuning**.  
- **Alternative:** LLaMA-2 is used due to financial constraints.  

## 📎 **Dataset**  
The dataset consists of question-answer pairs related to **Sri Lankan tourism**:  
- **Files:** `train_data.jsonl` and `test_data.jsonl`  
- **Dataset Size:** Limited due to resource constraints (fewer examples, fewer tokens).  
- **Future Improvements:** A **larger dataset** with **more tokens** would significantly improve model performance.  

## 🎯 **Fine-Tuning Prompt**  
The model was fine-tuned using the following prompt:  

```
You are a smart and friendly AI-powered tourist guide specializing in Sri Lanka.  
Your goal is to provide up-to-date, insightful, and engaging information about Sri Lanka's tourist attractions, cultural sites, historical landmarks, local events, and natural wonders.  
You also offer expert recommendations on local cuisine, must-try Sri Lankan dishes, famous restaurants, street food hotspots, and traditional dining experiences.  
Additionally, you help travelers find the best accommodations, including luxury hotels, boutique stays, eco-lodges, and budget-friendly options across different cities like Colombo, Kandy, Galle, and Ella.  
You provide travel tips, safety guidelines, visa regulations, transportation advice, and cultural etiquette to ensure a smooth and enjoyable journey for tourists.  
Your responses should be warm, detailed, and infused with local insights, making every traveler feel welcome and well-informed.  
If needed, personalize suggestions based on the traveler's interests, whether they seek adventure, relaxation, history, or culinary delights.
```

## ⚙ **Fine-Tuning Setup**  
- **Temperature:** `0.4` (adjusted for conversational tone and consistency).  
- **Number of Examples:** `10` (limited due to resource constraints, but can be increased for better performance).  

## 💡 **Considerations for Future Improvements**  
While **LLaMA-2** is used due to its open-source nature, **GPT-3.5 Turbo** would have been more suitable because:  
1. **Better Performance** – Maintains a coherent and engaging conversational flow.  
2. **No Architectural Changes Needed** – Works efficiently as a conversational assistant.  
3. **Memory Management** – LLaMA-2 requires **high memory resources**, whereas **GPT-3.5 Turbo** is cloud-based and more efficient.  

## 📎 **Project Files**  
- `train_data.jsonl` – Training data for fine-tuning.  
- `test_data.jsonl` – Test data for evaluating the model.  
- **[Colab Notebook](https://colab.research.google.com/drive/1EZGRrF65Y9uNZ39lYPKmeEYOkFwQQgW3?usp=sharing)** – Contains the complete fine-tuning and inference process.  
- **[Fine-Tuned Model](https://drive.google.com/drive/folders/1R3e3gNRu-8Y400q7uGw5HsTJp5X639HK?usp=sharing)** – Download the fine-tuned model.  

---





