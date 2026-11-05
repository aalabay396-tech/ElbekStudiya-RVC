# 🎙️ Elbek Studiya — RVC Voice Model Trainer

<div align="center">

![Elbek Studiya](https://img.shields.io/badge/Elbek%20Studiya-RVC%20Trainer-e94560?style=for-the-badge&logo=microphone)
![Gradio](https://img.shields.io/badge/Gradio-UI-orange?style=for-the-badge)
![ngrok](https://img.shields.io/badge/ngrok-Tunnel-blue?style=for-the-badge)
![Colab](https://img.shields.io/badge/Google%20Colab-GPU-yellow?style=for-the-badge&logo=googlecolab)

**Ovozingizni yuklang → Model nomini kiriting → Train → ZIP yuklab oling**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aalabay396-tech/ElbekStudiya-RVC/blob/main/ElbekStudiya_RVC_Trainer.ipynb)

</div>

---

## ✨ Xususiyatlar

- 🎨 **Chiroyli Gradio UI** — qoʻngʻir va qizil ranglar bilan
- 🔗 **ngrok + Gradio share** — ommaviy havola avtomatik chiqadi
- 📦 **Avtomatik ZIP** — `.pth` + `.index` fayllar bitta arxivga
- 🔁 **Bir necha model** — har safar yangi ism bilan yangi model
- ⚡ **Google Colab GPU** — T4 bepul GPU da ishlaydi
- 🇺🇿 **O'zbek tilli** interfeys

---

## 🚀 Ishlatish

### 1. Colabda oching

Yuqoridagi **"Open in Colab"** tugmasini bosing yoki:

```
https://colab.research.google.com/github/aalabay396-tech/ElbekStudiya-RVC/blob/main/ElbekStudiya_RVC_Trainer.ipynb
```

### 2. GPU yoqing

```
Runtime → Change runtime type → Hardware accelerator: T4 GPU → Save
```

### 3. Barcha katakchalarni ishga tushiring

```
Runtime → Run all   (yoki Ctrl+F9)
```

### 4. Gradio havolasiga kiring

2-katakcha oxirida:
```
Running on public URL: https://xxxxxxxx.gradio.live
```
Shu havolani bosing!

---

## 🎛️ Interfeys

```
┌─────────────────────────────────────────────────────────────────┐
│          🎙️  Elbek Studiya  RVC Model Trainer                   │
│           ⚡ Retrieval-based Voice Conversion v2                 │
├──────────────────────────┬──────────────────────────────────────┤
│  📋 Model sozlamalari    │  📊 Natija va jarayon                │
│                          │                                      │
│  🏷️ Model nomi:          │  📜 Jarayon jurnali:                │
│  [sarvar_ovozi_____]     │  ✅ Dataset tayyor                   │
│                          │  ⏳ Ovoz qayta ishlanmoqda...        │
│  🎤 Ovoz fayllari:       │  🎵 Pitch chiqarilmoqda...           │
│  [Fayllarni yuklang  ]   │  🧠 Xususiyatlar...                 │
│                          │  🏋️ Model o'qitilmoqda (100 ep)     │
│  ⚙️ Kengaytirilgan:      │  📑 Index yaratilmoqda...            │
│  Epoch:  [100 ───────]   │  🎉 TAYYOR!                         │
│  SR:     ○ 40k  ○ 48k    │                                      │
│  Pitch:  [rmvpe ▾]       │  📦 model_ElbekStudiya.zip          │
│  Batch:  [4   ───────]   │  [⬇️ Yuklab olish]                  │
│                          │                                      │
│  [🚀 O'QITISHNI BOSHLASH]│                                      │
└──────────────────────────┴──────────────────────────────────────┘
```

---

## 📦 ZIP fayl tarkibi

| Fayl | Tavsif |
|------|--------|
| `model_nomi_e100.pth` | Asosiy model (ovoz xususiyatlari) |
| `added_IVF_..._model.index` | FAISS qidiruv indeksi |

---

## ⚙️ Sozlamalar

| Sozlama | Tavsiya | Tavsif |
|---------|---------|--------|
| **Epoch** | 100–300 | Ko'proq = yaxshiroq (lekin vaqt ko'proq) |
| **Sample Rate** | 40000 | 40k standart, 48k premium |
| **Pitch algo** | rmvpe | Eng aniq pitch chiqarish |
| **Batch size** | 4–8 | GPU xotirasiga qarab |
| **Save every** | 10 | Har 10 epochda checkpoint |

---

## 💡 Maslahatlar

> **Dataset sifati** — 10–20 daqiqa sifatli, shovqinsiz ovoz yaxshiroq natija beradi

> **ngrok token** — [dashboard.ngrok.com](https://dashboard.ngrok.com/get-started/your-authtoken) dan bepul token oling. Token bo'lmasa ham Gradio `.gradio.live` havolasi chiqadi.

> **Colab sessiyasi** — Sessiya uzilsa, modellar saqlanmaydi. Google Drive ga ulab qo'ying!

---

## 🔗 Model ishlatish mumkin bo'lgan joylar

- [RVC Simple UI (HuggingFace)](https://huggingface.co/spaces/r3gm/RVC_HF)
- [AICoverGen](https://github.com/SociallyIneptWeeb/AICoverGen)
- [w-okam.com](https://w-okam.com)

---

<div align="center">

Made with ❤️ by **Elbek Studiya** | Powered by [RVC-Project](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI)

</div>
