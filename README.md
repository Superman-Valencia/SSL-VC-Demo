# <p align="justify"> Voice Conversion using Self-Supervised Features and a Multi-Constraints Disentanglement Strategy

# ABSTRACT
<p align="justify"> Voice conversion (VC) is challenging, especially in unseen scenarios.
This paper proposes a VC model using self-supervised features and a multi-constraints disentanglement strategy.
First, the self-supervised features extracted by specific layers of pre-trained speech processing model WavLM are
employed as input for the speaker encoder and the content encoder to improve the model's generalization and simplify
their architectures. Second, a multi-constraints disentanglement strategy is proposed to remove redundant information
in pre-trained features. Specifically, the Siamese content loss is adopted to mitigate the speaker information leakage
issue in content encoding. The margin speaker loss based on AM-Softmax is introduced to alleviate the problem of overlap
and fuzzy boundaries between different speakers. The pitch loss and the mel-spectrogram reconstruction loss are adopted
to ensure the converted speech's quality. Besides, the generalization strategy employed during the training stage further
makes the generated speech more realistic. Experimental results on the VCTK corpus demonstrate that the proposed model achieves
excellent performance in objective and subjective evaluations under both seen and unseen scenarios.</p>

The following is the overall model architecture.
<div align="center">
  <img src="images/proposed_model_revise.jpg" width="80%">
  <p>Fig.1: The overall architecture of the proposed model.</p>
</div>

# DEMO
For the converted samples, you can visit [the demo page](https://superman-valencia.github.io/SSL-VC-Demo/).
