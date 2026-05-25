# ENIGMIA HACKATHON 2026

![ENIGMIA 2026](https://github.com/user-attachments/assets/c9050819-7b4f-44d6-bb78-ef8725456ee9)

Built during **ENIGMIA 2026**, a 48-hour hackathon challenging teams to build solutions that help culture coexist with AI rather than be consumed by it.

---

# Diwani

Diwani is a mobile application built to protect and transmit Algerian visual culture in an era where AI risks standardizing and erasing local artistic identity. Named after the Diwani calligraphic script rooted in Islamic art tradition, the app serves as a living archive of Algerian painting, folk art, and artistic techniques — powered by AI, but driven by human heritage.

## About

**Link to our MVP app:** [Google Drive Folder](https://drive.google.com/drive/folders/1LOt9jrZywOkAd2Bh6lPBSTIMvzShFPNo?usp=sharing)

### Demo

![Diwani Demo](https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExeHJlajB4YWVqM2t2Ymh0bnA1ZHdnN3FkZTdobmNzOXd0ejh1cXF5byZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/L1PNLR4o35cl8LESdL/giphy.gif)

![Feature Showcase](https://github.com/user-attachments/assets/8b53a0cb-7e79-4757-9a25-daf8572bcb74)

---

## What Diwani Does

- **Artwork Recognition** — Point your camera at a painting or motif and instantly identify its style, period, and cultural origin
- **Artist Archive** — Discover Algerian artists past and present, their techniques, influences, and works
- **Learn to Paint Algerian** — Step-by-step guides teaching the fundamentals of Algerian artistic traditions (Amazigh patterns, arabesque, Msila pottery motifs, and more)
- **Alternatives** — AI suggests how to recreate traditional techniques with accessible modern materials
- **Community Contributions** — Artists and enthusiasts submit works, stories, and techniques to grow the archive

---

## Tech Stack

| Layer | Technology |
|---|---|
| Mobile Framework | React Native (Expo) |
| Database & Auth | Supabase |
| AI & Image Processing | Gemini API (Vision + Text) |
| Image Storage | Supabase Storage |
| Deployment | Expo Go / EAS Build |

---

## AI Architecture

```
[Reference Algerian Artwork]        [User's Photo / Subject]
            ↓                                   ↓
     Prompt 1:                         Image Processing
     Style Extraction                  (resize, normalize)
     via Gemini API                             ↓
            ↓                          Subject features
     Style descriptor                  extracted
     stored as text     ──────────→            ↓
                                       Prompt 2: Fusion
                                       via Gemini API
                                       "Apply this Algerian
                                       style to this subject"
                                                ↓
                                  ✦ Output: subject redrawn
                                    in Algerian artistic style
```

---

## Team

**Artistote** — ENIGMIA 2026


| | Name | GitHub |
|---|---|---|
| <img src="https://github.com/abderrahmaneosmani.png" width="40" height="40" style="border-radius:50%"/> | Abderrahmane Osmani | [@abderrahmaneosmani](https://github.com/abderrahmaneosmani) |
| <img src="https://github.com/61j3t.png" width="40" height="40" style="border-radius:50%"/> | Member 2 | [@61j3t](https://github.com/61j3t) |
| <img src="https://github.com/asmaAouadi.png" width="40" height="40" style="border-radius:50%"/> | Asma Aouadi | [@asmaAouadi](https://github.com/asmaAouadi) |
| <img src="https://github.com/zetoo007.png" width="40" height="40" style="border-radius:50%"/> | Member 4 | [@zetoo007](https://github.com/zetoo007) |

---

## Getting Started

### Prerequisites
- Node.js 16+
- Expo CLI
- Supabase account
- Google Gemini API key

### Installation

1. Clone the repository
```bash
git clone https://github.com/aristote-enigmia/Demo.git
cd Demo
```

2. Install dependencies
```bash
npm install
```

3. Set up environment variables
```bash
cp .env.example .env.local
```

4. Start the development server
```bash
expo start
```

---

## Contributing

We welcome contributions! Please feel free to submit a Pull Request.

## License

MIT License — See [LICENSE](LICENSE) for details.
