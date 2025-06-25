# 🧠 Language Model Integration with Wav2Vec2 for Oromo and Amharic

This project boosts **Wav2Vec2** speech recognition models using a **KenLM 5-gram language model**, enhancing decoding quality for **low-resource African languages** such as Oromo and Amharic.

---

## 🎯 Objectives

- Download or prepare `.arpa` language models.
- Build a binary KenLM (`.bin`) for fast decoding.
- Use `pyctcdecode` to attach the LM to Wav2Vec2.
- Save the enhanced `Wav2Vec2ProcessorWithLM`.
- Upload the processor to Hugging Face with Git LFS.

---

## 🧰 Dependencies

Install required libraries:

```bash
pip install datasets transformers torchaudio librosa jiwer evaluate pyctcdecode \
            huggingface_hub wandb matplotlib seaborn accelerate

# KenLM and build tools
sudo apt install build-essential cmake libboost-all-dev zlib1g-dev libbz2-dev liblzma-dev git-lfs
