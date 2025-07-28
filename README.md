#  Problem Statement
In any organization that handles customer service, support tickets can pile up quickly. These tickets come in as free-form text, and it's up to the support team to figure out what each one is about—whether it's a billing issue, a technical problem, an account access request, or something else. Manually reading and tagging each ticket takes time and can lead to mistakes, especially when the volume is high.

The goal of this project is to automate that tagging process using large language models (LLMs). Instead of relying on rule-based systems or manual effort, we’ll use models that can understand the content of each support ticket and assign relevant tags to it.

We'll experiment with a few different methods:

Zero-shot learning, where the model guesses the category without seeing any training examples.
Few-shot learning, where we give the model a few examples to learn from in the prompt.
Fine-tuned models, where we train the model on a labeled dataset to make it more accurate.

In the end, the system should be able to return the top 3 most likely categories for any incoming ticket. This would make it easier for support teams to prioritize and handle issues more efficiently.
