# [[M2L2025](https://www.m2lschool.org/home)] Tutorial 5: Diffusion Models

**Authors:** Gabrijel Boduljak, James Thornton

In this tutorial, we’ll build the theoretical foundation for understanding continous-time diffusion models. The key idea is simple but powerful: we can gradually corrupt real data with noise using a forward process, and then learn to reverse this corruption process step by step to generate new data samples from pure noise. We’ll start by introducing stochastic differential equations (SDEs) and how they let us formalize this forward noising process. Then we’ll see how the reverse process can recover the data, and why we need to approximate it with a neural network trained via denoising score matching (DSM). Finally, we’ll explain one of the most remarkable features of diffusion models: their guidance ability. This allows us to steer generation toward desired outcomes. We’ll explore and explain state-of-the-art classifier-free guidance and demonstrate how it can be used to generate specific digits from the MNIST dataset. We will also show how to incorporate classifier-free guidance in the state-of-the-art diffusion architecture, DiT. In the optional part, we will explore a connection between flow matching (state-of-the art generative modelling paradigm) and score-based diffusion.

By the end, you’ll have a clear picture of :

1. What diffusion models actually learn?
2. How to train diffusion models?
3. How to sample from diffusion models, potentially guiding the sampling process towards the desired outcome?

Tutorial outline:

1. Practical 1. Fundamentals of Score-Based Diffusion Models (basic level)
2. Practical 2. Controllable (Image) Generation (intermediate/advanced level)
3. [Optional] Practical 3.: Deterministic Sampling and Connection Between Flow Matching and Score-Based Diffusion Models (advanced level)
   
Diffusion models can get pretty math-heavy, so we’ve put together a separate Theory notebook to go along with the exercises. You’ll also find some optional material in there if you want to dive deeper on your own.

---

Theory Recap: [![Open In 
Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/M2Lschool/tutorials2025/blob/master/5_diffusion/%5BM2LS_2025%5D_Theory_recap.ipynb
)

#### Part 1:
Tutorial: [![Open In 
Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/M2Lschool/tutorials2025/blob/master/5_diffusion/%5BM2LS_2025%5D_Fundamentals.ipynb)


#### Part 2:
Tutorial: [![Open In 
Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/M2Lschool/tutorials2025/blob/master/5_diffusion/%5BM2LS_2025%5D_Conditional_Generation.ipynb)


#### Part 3:
Tutorial: [![Open In 
Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/M2Lschool/tutorials2025/blob/master/5_diffusion/%5BM2LS_2025%5D_Optional.ipynb)
