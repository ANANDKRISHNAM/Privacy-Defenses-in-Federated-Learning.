# Defending Against Generative Gradient Leakage Attack with Gradient Quantization

## Introduction

Federated Learning (FL) is a decentralized machine learning approach where model training occurs on local devices or servers, with only model updates, called gradients, shared with a central server. However, this collaborative paradigm introduces privacy risks, one of which is Generative Gradient Leakage (GGL).

## Understanding Generative Gradient Leakage (GGL)

Generative Gradient Leakage (GGL) is a privacy attack in FL where adversaries exploit the gradients shared during model updates to infer sensitive information about the training data. Unlike traditional attacks that focus on direct data extraction, GGL leverages generative models, such as Generative Adversarial Networks (GANs), trained on public image datasets, to reconstruct private data from the gradients.
 
## The Defense: Gradient Quantization

To mitigate the risk posed by GGL, gradient quantization is proposed as a defense mechanism. Gradient quantization reduces the precision of gradients by mapping them to a smaller set of discrete values. This process introduces noise and distortion into the gradient updates, making it significantly more challenging for adversaries to extract meaningful information from them.

By quantizing gradients, the fine-grained details that could potentially leak sensitive information about the training data are obfuscated. As a result, gradient quantization serves as an effective defense against GGL, bolstering the privacy and security of FL systems.

## Conclusion and Result

Generative Gradient Leakage (GGL) poses a serious threat to the privacy of federated learning systems, allowing adversaries to infer sensitive information from shared gradients. To combat this threat, gradient quantization provides a robust defense mechanism by reducing the precision of gradients and mitigating the risk of data leakage. By adopting such defensive strategies, FL systems can enhance their resilience against privacy attacks and safeguard the confidentiality of sensitive data.


<img width="332" alt="image" src="https://github.com/ANANDKRISHNAM/Privacy-Defenses-in-Federated-Learning./assets/40604290/bc678445-2d61-45a8-be09-c64778cd611e">

<img width="892" alt="image" src="https://github.com/ANANDKRISHNAM/Privacy-Defenses-in-Federated-Learning./assets/40604290/59ee705a-ff15-4997-b8be-8d98257d58fc">

My Novelty:

Prevent Reconstruction (GGL Attack) but still collaberative learning happens
<img width="855" alt="image" src="https://github.com/ANANDKRISHNAM/Privacy-Defenses-in-Federated-Learning./assets/40604290/d47d4899-182e-4905-9c99-936eaea5e72e">
