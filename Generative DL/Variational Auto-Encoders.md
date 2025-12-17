# Variational Autoencoders (VAE) : Conceptual Guide

## 1. Overview and Motivation
- Overview: What problem a VAE is trying to solve  
- Limitations of a standard Autoencoder  
- The need for a structured and continuous latent space  

## 2. Conceptual Shift in Representation
- Shift from deterministic encoding to latent explanations  
- What the VAE encoder is really trying to answer  

## 3. Encoder and Latent Parameters
- Encoder architecture and feature extraction  
- Latent parameters: μ (Mean) and σ (Scale)  
- Interpreting μ and σ for a single input  

## 4. Latent Space and Sampling
- Latent distribution per input image  
- Introducing sampling in latent space  
- Role of ε (Epsilon) in controlled variation  
- Reparameterization trick  

## 5. Decoder and Reconstruction
- Decoder architecture and reconstruction process  
- Reconstruction loss and its role  

## 6. Loss Function and Latent Space Discipline
- Latent space regularization (KL Divergence)  
- How reconstruction loss and KL loss work together  

## 7. Training Dynamics and Emergent Structure
- Training dynamics and backpropagation behavior  
- Emergence of meaningful regions in latent space  

## 8. Using a Trained VAE
- Inference on new data  
- Generation from latent space  
- Applications, strengths, and limitations of VAEs
