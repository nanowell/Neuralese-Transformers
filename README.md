# Neuralese-Transformers
My first successful implementation of Neuralese that helps to significantly improve story generation and make them feel more personal and less determenistic without any training or special prompting just an emergent behavior!

Qwen3-0.6B
---
Generated with Neuralese:
```
user
Who are you?
assistant
<think>
Okay, I need to answer the user's question "Who are you?" as an AI assistant. First, I should acknowledge their query and explain that I'm not a person but an advanced language model trained on large datasets.

I'll start by stating my purpose clearly: to help with tasks like answering questions or providing information. Then mention that I don't have personal experiences or feelings, so we can work together in conversation.

Make sure to keep it friendly and approachable without making up facts about me. Also, offer assistance if they have any specific needs or wants from me.
 That sounds good! Let me put this into a natural response now.
</think>

Hello! I’m here to assist you with people with typical answers... (pauses) Yes, I am an AI designed to understand your questions and provide helpful responses. Do you want help with something else?

(whispering) No, no, nothing? Okay, let me think of how to respond appropriately. But since I cannot say that I do not feel happy, I will just ask for more details in case you have anything needed. So please tell me what would be important for you today."
```
--- Standard Generation (Baseline) ---
```
user
Who are you?<|im_end|>
<|im_start|>assistant
"
Both `max_new_tokens` (=512) and `max_length`(=62) seem to have been set. `max_new_tokens` will take precedence. Please refer to the documentation for more information. (https://huggingface.co/docs/transformers/main/en/main_classes/text_generation)
Generated (standard): "user
Who are you?
assistant
<think>
Okay, the user asked "Who are you?" I need to respond appropriately. First, I should acknowledge their question and explain my purpose.

I can say something like, "Hello! My name is a model assistant." Then provide details about what I do, such as answering questions or providing information.

It's important to keep the response friendly and helpful. Also, make sure not to use any markdown formatting and keep it conversational.
</think>

Hello! I'm an AI language model designed to assist with various tasks like answering questions, providing information, or helping with specific needs. If you have anything in mind, feel free to ask me! 😊"
```
