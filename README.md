# Finetuning with UnSloth AI

## What is fine tuning in LLMs?

In simple terms, it's adjusting a general tool/chat bot to talk about things we want it to talk about more often.

It's similar to recommendation systems as in:

A fresh content feed (facebook,youtube,reddit,etc) will have a wide variety of topics but as you use it. You will get a more personalized feed. If you watch minecraft, you get more minecraft videos but you can actively search outside of that.

**So**

Fine tuning is augmenting/adjusting the weights of an existing model by inputting our own context specific knowledge to perform better in a particular area.

## Why finetune?

Simply put. Rather than building a system from the ground up, we just adjust an existing system for our needs.

It's like having a table that's a bit too short for your liking. You could get a new table that's just right for you or you can just slap a block of wood under the legs to make it slightly taller.

Same principle.

Theoretically, this grants most people the capability to have a working LLM assistant, tailored to their use case, with minimal investment as they can rely upon the reliability of the original model.

## How to finetune?
There's a variety of ways to do it. Conceptually, it's just adding more data to a dataset. It's just training on top of training, there is no difference.

So all models that have been built from the ground up can be fine tuned. This comes with clear costs which are enumerated within this blog post in their key takeaways

https://encord.com/blog/training-vs-fine-tuning/

So if you understand how to train a model from scratch, you can fine tune a model.

If you don't. No worries, we'll use Unsloth AI as a learning tool to help you get to terms with the process.

## Further reading
In your personal searches about the topic, you'll come up with a variety of topics such as RAGs (Retrieval-Augmented Generation)

To put it in simple terms. When you ask ChatGPT questions, it gives you the most probably answer within that context.

It "looks up" the correct answer for your question, however it's source is "trust me bro"

RAGs actually look it up with citations.

You can read further in these blog posts
https://www.datacamp.com/tutorial/rag-vs-fine-tuning
https://www.datacamp.com/tutorial/fine-tuning-large-language-models

## Unsloth Guide
In the event that this guide becomes outdated (incredibly likely within 2 years). PLEASE RTD (READ THE DOCUMENTATION). 

I understand some documentation is terrible in explaining anything but unsloth created a wonderful primer on how to use their tool, as well as explaining what each component does.

https://docs.unsloth.ai/basics/tutorial-how-to-finetune-llama-3-and-use-in-ollama

For this guide, we'll be using google colab, but this can be done in any python environment. the benefits of using google colab is that the fine tuning of the model is not dependent on your system since it's processed on one of google's machine (or in the cloud).

To use this locally, it'll be left as an exercise to the reader due to large segments of the code base being easily transferrable to a local python venv

