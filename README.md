# G2SC

The officialPytorch implementation for the paper "GAI-Driven Knowledge Distillation for Personalized Semantic Communications via Federated Learning".

![SC_system_model](figures/SC_system_model.jpg)



## Introduction

Semantic communication (SC) combines advanced artificial intelligence (AI) with traditional wireless communication to accommodate various task-oriented scenarios. However, with the growing requirements for personalization, users expect customized and specialized communication services. Federated learning (FL) attracts attention as a technology that simultaneously ensures personalized services and privacy protection, yet it remains incompatible with the SC architecture. Specifically, SC requires additional consideration of the impact of the physical channel, which means that changes in channel assumptions would necessitate retraining the model. However, under FL conditions, such a cost is unacceptable. A key insight is that channel coding can be shared across all SC models, whereas user knowledge is unique. Therefore, we decouple personalized demand from general functions within SC and propose a two-stage SC framework, named distillation-to-SC (D2SC). In the first stage, we employ FL to extract knowledge from private user data by knowledge distillation. To elaborate, we employ pretrained generative AI as the teacher, which has strong semantic modeling capability, to transfer the knowledge to the student. In the second stage, since the student model contains specialized knowledge for each user, we can reuse it by incorporating the physical channel and semantic decoding. Moreover, we design a dual transmission optimization to address the adverse effects of channel fading on semantic transmission. Extensive experiments demonstrate that D2SC achieves optimal performance across multiple SC tasks and effectively handles both unknown channel interference in transmission and imbalanced data distributions.



## Code

The completely code and trained model weights and execution logs are released as open source after the paper is accepted.
