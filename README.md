# vae-wgan-audio
A VAE-WGAN + HIFI-GAN (pre-trained) model for audio generation.

## Main Results
- **Reconstruction**: Model reconstructs male voices well but introduces artifacts in female voices; spectrograms are sharp but harmonic dynamics are often simple (flat lines).
- **Unconditional generation**: Outputs resemble mumbling rather than intelligible digits; Thus latent space is not perfectly regularized.
- **Interpolation**: Smooth transitions are visible in spectrograms, but audio quality degrades, especially when interpolating with a high voice.

## Repository Structure
- `vae_gan_audio.ipynb` – Colab notebook with implementation and experiments.
- `recon_gen/` – audio samples from reconstruction of real spectrograms.
- `random_gen/` – samples from unconditional generation.
- `interpolated_gen/` – samples from latent space interpolation between two speakers.

