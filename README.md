# CLIP-VQGAN

The aim of this project is to create a codebook utilizing the pre-existing CLIP model, thus eliminating the need to train the encoder in VQGAN. Additionally, leveraging the strong alignment between text and image contents, the goal is to potentially reduce the training time of the transformer in conditional image generation.

Ideally, the VQGAN's decoder can directly derive from established diffuse models based on the CLIP text encoder, requiring only fine-tuning of the codebook for smaller or more general datasets, given the extensive training dataset that CLIP has undergone.

However, a limitation arises from the restricted image resolutions of current open-source CLIP models. This limitation may result in insufficient information capture when images are segmented into patches and processed through the CLIP model to generate the codebook embeddings.


