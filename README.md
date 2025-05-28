# LLMFinetuning


| Day  | Project                                       | Model                                | Dataset                           | Goal                                          |
| ---- | --------------------------------------------- | ------------------------------------ | --------------------------------- | --------------------------------------------- |
| 3-4  | 🧠 **Fine-tune GPT2 on Custom Chat Dataset**  | `gpt2`                               | Your own Q\&A or dialogue dataset | Learn full fine-tuning                        |
| 5    | 🔁 **Instruction Tuning TinyLlama**           | `TinyLlama/TinyLlama-1.1B-Chat`      | Alpaca-style JSON                 | Practice SFT (Supervised Fine-Tuning)         |
| 6    | 🔧 **Apply LoRA on LLaMA2 or Mistral**        | `mistralai/Mistral-7B-Instruct-v0.1` | Small instruction dataset         | Learn PEFT with 4-bit quant                   |
| 7    | 📊 **Fine-tune T5 for Text Summarization**    | `t5-small`                           | CNN/DailyMail (or custom)         | Learn encoder-decoder tuning                  |
| 8–10 | 🤖 **Train a Sentiment Classifier with BERT** | `bert-base-uncased`                  | IMDB                              | Learn classification with HuggingFace Trainer |


1. How much data do you need to fine-tune?
    LIMA paper shows as low as 1k carefully curated examples. Focus on curating and quality. 
2. How do you find more datasets? 
    Instruction Backtranslation: You do not lack datasets. You lack QA pairs. Prompt a LLM to convert your documents and curate them. 
3. How to create stronger domain specific models? 
    Use a larger model to add Chain-of-Thought to your datasets
4. How to curate your examples? 
    Tinystories shows when working on a new domain, utilize a progressive learning. Create a curriculum for your models. 
5. Bonus approach for curating: 
    Textbooks are all you need shows you should can also curate exercises for your models as part of the curriculum. 
6. Toolformer: One of the first papers to unlock API calling. 
    The paper technically created the field of AI agents-it's exciting to think more great ideas are around the corner. 
7. How can you improve tool calling? 
    Gorilla paper shows by adding API documentation to your examples
8. One step further for tool calls: 
    ToolLLM paper shows combining a DFS like algorithm to curate synthetic annotations.


https://github.com/meta-llama/synthetic-data-kit/tree/main/use-cases/awesome-synthetic-data-papers
