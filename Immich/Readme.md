# Immich - Self-Hosted Photo Server

A self-hosted Immich server running on old hardware, using an NVIDIA GPU for CUDA-accelerated machine learning.

## Why Immich?

🔒 Private, self-hosted photo storage

📱 Automatic phone backup

👤 Face detection & recognition

🔎 Smart search and organization

⚡ NVIDIA CUDA acceleration

♻️ Reusing old hardware

## Hardware
Old PC

├── SSD → OS + Docker + Redis

├── HDD → Photos & Videos

└── NVIDIA GPU → CUDA / Machine Learning


Keeping Redis and the application stack on the SSD helps responsiveness, while the large HDD provides inexpensive storage for the photo library.

## CUDA

The NVIDIA GPU is passed to Immich's Transcoding and Machine Learning container for accelerated ML workloads such as face detection.

nvidia-smi

## Storage
SSD

├── OS

├── Docker

└── Redis / Immich services

HDD

└── 📸 Photos & Videos


Self-hosted ≠ backed up. Keep a separate backup of important photos.

## Deployment

Immich runs with Docker Compose.

https://immich.app/docs

## Goal

Turn old hardware into a private Google Photos alternative - CUDA-powered face detection, SSD-backed services, and photos stored on large HDDs.
