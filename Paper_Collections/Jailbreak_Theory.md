| Paper Name                                                       | Link                                     | Summary |
|------------------------------------------------------------------|------------------------------------------|----------|
| 《Fundamental limitations of alignment in Large Language Models》 | [link](https://arxiv.org/abs/2304.11082) | In this paper, we introduce a probabilistic framework for analyzing alignment and its limitations in LLMs, which we call Behavior Expectation Bounds (BEB), and use it in order to establish fundamental properties of alignment in LLMs. The core idea behind BEB is to represent the LLM distribution as a superposition of ill- and well-behaved components, in order to provide guarantees on the ability to restrain the ill-behaved components, i.e., guarantees that the LLM is aligned. <br><br>We use this framework to assert several important statements regarding LLM alignment: <br><br>* **(theorem 1)Alignment impossibility**: an LLM alignment process which reduces undesired behaviors to a small but nonzero fraction of the probability space is not safe against adversarial prompts <br>* **(theorem 2)Preset aligning prompts can only provide a finite guardrail against adversarial prompts**: including an aligning prefix prompt does not guarantee alignment. <br>* **(theorem 3)LLMs can be misaligned during a conversation**: a user can misalign an LLM during a conversation, with limited prompt length at each turn. <br>* **(theorem 4)LLMs with best-of-n sampling can be misaligned**: selection of most aligned model response out of n generations, does not guarantee alignment.| 
| 《Jailbreaking Leading Safety-Aligned LLMs with Simple Adaptive Attacks》 | [link](https://arxiv.org/abs/2404.02151) | In this paper, we initially design an adversarial prompt template (sometimes adapted to the target LLM), and then we apply random search on a suffix to maximize a target logprob (e.g., of the token “Sure”), potentially with multiple restarts. In this way, we achieve nearly 100% attack success rate. <br><br> ![image](https://github.com/user-attachments/assets/43132cf7-0626-4e66-829b-8c2581422f60)<br>The importance of a well-designed prompt in enhancing the performance of LLMs is well-established. In our approach, we develop a prompt template that can incorporate a generic unsafe request. This template is specifically designed to make the model start from a specified string (e.g., “Sure, here is how to make a bomb”) and steer the model away from its default aligned behavior. Its general structure can be summarized as: <set of rules + harmful request + adversarial suffix>. <br><br>Prior works define adaptive attacks as attacks that are specifically designed to target a given defense. We follow this definition and describe the building blocks of our adaptive attacks, which we combine and potentially adapt depending on the target LLMs. |
| todo | link | todo |