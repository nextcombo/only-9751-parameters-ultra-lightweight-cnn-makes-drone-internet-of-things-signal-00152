# Only 9751 parameters! Ultra-lightweight CNN makes drone Internet of Things signal modulation recognition "fast and accurate" [with Python code]

Only 9751 parameters! Ultra-light CNN enables drone IoT signal modulation recognition to be "fast and accurate". In today's rapid development of drone IoT (IoUAV), automatic modulation classification (AMC) has become a core technology in communication security, interference management, and spectrum perception. However, traditional deep learning models are large in size and consume substantial computational resources, making them unfeasible to run on the limited computing power of drones.

Recently, a study published in the IEEE IoT Journal offers a perfect solution - ultra-light convolutional neural networks (CNNs) that achieve high accuracy and low latency modulation recognition with minimal model volume, specifically designed for resource-constrained drone systems.

I. Research Background: Challenges in Drone-end Modulation Recognition
Automatic modulation classification (AMC) can help drones identify signal types, resist interference, and optimize communication quality, serving as the "signal eyes" of drone IoT.

While AMC based on deep learning is highly accurate, it faces two major challenges:
★ The model parameters are numerous and voluminous, which cannot be stored or run on the drone end.
★ The computational complexity is high, leading to slow inference and failing to meet real-time requirements.
Existing lightweight methods either suffer from significant loss in accuracy or complex structures, making it difficult to find a balance between "lightweight" and "accurate".

To address this, the team proposes an ultra-light CNN architecture, focusing on: extremely small parameters, ultra-low computation, real-time inference, and maintaining accuracy.

II. Core Methodology: Ultra-Light Modulation Recognition Framework
The framework does not pile on complex structures but instead designs compact structures and employs lightweight techniques to push the model to its limits while preserving performance. It consists of three core modules plus two optimization strategies.
1. Three Core Modules:
★ IQ Channel Fusion Module (IQCF):
Utilizes complex value convolution to directly mine the correlation between the I/Q channels of signals, more aligned with the characteristics of communication signals than traditional real-value convolution, thoroughly understanding the signal features at the outset.
★ Feature Mining and Dimensionality Reduction Module (FMDR):
Stacks 6 levels of lightweight structure, integrates deep separable convolution, channel shuffling, and channel attention. It simultaneously enhances feature depth and dramatically reduces dimensions, achieving a 50% reduction in computational load while improving resolution.
★  
Cross-Layer Feature Fusion Module (CLFF)
Weighted fusion of the output features from the 4th to 6th layers of FMDR, taking into account both high and low signal-to-noise ratios, ensures that the model can maintain its robustness in weak signal environments.
2. Two key optimizations ★
Rotational Data Augmentation: Expand the training samples by a factor of four, enhancing robustness and generalization.
★  
Adaptive learning rate: If the validation loss does not decrease, the learning rate will be automatically reduced to prevent overfitting and ensure more stable convergence.
III. Experimental Results: Lightweight to the extreme, strong to surprise. The research conducted a comprehensive comparison on the public dataset RML2016.10a, and the results were very impressive:
1. Accuracy rivals large models★
After data augmentation, the average classification accuracy reached 62.47%.
★  
Accuracy exceeds 92% under high signal-to-noise ratio (≥6 dB)
★  
Only 0.08% lower than the top-tier large model MCLDNN, with almost identical accuracy.
2. Volume crushing all competitors★
Total parameters only 9751 (less than 10,000).
★  
It is 1/40 of MCLDNN and 1/7 of PET-CGDNN, which can be considered one of the smallest AMC deep learning models currently.
3. Real-time inference at the edge on drone-level edge devices: Raspberry Pi 4B
★  
Single-sample inference only 0.775 ms
★  
Far below the 1ms latency threshold, meeting the real-time signal processing needs of drones.
The inference on GPU is even faster to 0.01 ms, and the cloud deployment is also efficient.
Ablative experiments prove that: recurrent convolution, channel attention, channel shuffling, cross-layer fusion, and adaptive learning rate, each component is actually improving performance.
IV. Research Conclusions and Future Directions: This study demonstrates that ultra-lightweight models can be fully implemented in drone Internet of Things for high-precision modulation recognition.
Through compact structure design, the best balance is achieved between parameters, computational load, inference speed, and classification accuracy, making it highly suitable for drones, edge devices, and IoT terminals with strict limitations on computing power and storage.
In the future, the team will also combine techniques such as pruning, quantization, and knowledge distillation to further create hardware-friendly ultra-light models, allowing intelligent signal recognition to truly be implemented on every drone terminal.

## Images

![Only 9751 parameters! Ultra-lightweight CNN makes drone Internet of Things signal modulation recognition "fast and accurate" [with Python code].](01.jpg)
![Only 9751 parameters! Ultra-lightweight CNN makes drone Internet of Things signal modulation recognition "fast and accurate" [with Python code].](02.jpg)
![Only 9751 parameters! Ultra-lightweight CNN makes drone Internet of Things signal modulation recognition "fast and accurate" [with Python code].](03.jpg)
![Only 9751 parameters! Ultra-lightweight CNN makes drone Internet of Things signal modulation recognition "fast and accurate" [with Python code].](04.jpg)
![Only 9751 parameters! Ultra-lightweight CNN makes drone Internet of Things signal modulation recognition "fast and accurate" [with Python code].](05.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
