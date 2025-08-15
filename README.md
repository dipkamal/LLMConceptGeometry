# The Geometry of Concepts: Probing Alignment and Orthogonality in Representation Space of LLMs

Submitted to **Mechanistic Interpretability Workshop at NeurIPS 2025**.

Understanding the internal workings of large language models (LLMs) is critical for ensuring their safety and reliability. While Representation Engineering (RepE) has shown that abstract concepts are represented as vectors in activation space, these are studied in isolation. We extend this research by investigating how the geometric relationships between concept vectors evolve across the layers of three popular LLMs: **Llama-3-8B-Instruct model**, **Qwen2.5-7B-Instruct** and **DeepSeek-R1-Distill-Llama-8B**. 

Our layer-wise analysis reveals a dynamic process of conceptual refinement. Concepts that are coarsely and often incorrectly associated in early layers are progressively refined into a more nuanced, orthogonal basis. While the overall trend held, the models displayed unique signatures reflecting their training.  
- For example, in **Llama-3-8B-Instruct model**, "honesty" and "politeness" begin with a strong anti-correlation (cosine similarity of -0.84), reflecting a simplistic bias that these concepts are opposites. However, in later layers, the model actively corrects this, pushing their representations toward orthogonality. 
- The **DeepSeek model** showed a different initial bias for "honesty" and "politeness" but still converged to orthogonality, whereas the **Qwen model** showed a persistent, weak entanglement between these social concepts not seen in the other models. 


Notebook folder consists of three jupyter notebooks for each LLM.

