# 🔥 Image Prompt Engineering  
Advanced research on structured prompt design for **selfies and photography** in generative AI.  
This repository provides a documented framework for building **high-accuracy, identity-preserving prompts** with clear sections (Scene, Clothing, Hair, Expression, Pose, Camera, Lighting, etc.).  

---

## 📖 About  
This repo is a **lite version** of my full documentation on *Image Prompt Engineering*.  
It focuses on creating prompts that generate **consistent, realistic, and context-aware images** while preserving reference identity across outputs.  

The framework includes:  
- 📷 **Selfie Prompt Sections** → with pose and shot details specific to handheld/selfie context.  
- 🎞 **Photography Prompt Sections** → structured prompts for wider photographic compositions.  
- ⚡ **Generative Prompt Conversion** → how to merge descriptive sections into a final cohesive prompt.  
- ✅ **Negative/Avoid Guidelines** → prevent unwanted distortions (plastic skin, elongated necks, oversharpening, etc.).

| Feature / Section                                                                               | v1.1 | v1.2 | v1.3 | v1.4 | v1.5 | v1.6 | v1.7 | v1.8 | v1.9 |              v2.0 (Selfie)              |
| ----------------------------------------------------------------------------------------------- | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :-------------------------------------: |
| Basic sections (Scene, Clothing, Hair, Expression, Camera, Lighting, Skin, Imperfections, Mood) |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |                    ✔️                   |
| Negative / Avoid rules                                                                          |      |      |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |                    ✔️                   |
| Selfie-specific flag (explicit arm/hand note)                                                   |      |      |      |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  | Merged naturally into “Selfie Sections” |
| Gaze direction in Expression                                                                    |      |      |      |      |      |      |      |      |      |                    ✔️                   |
| Depth cues / surface details in Scene                                                           |      |      |      |      |      |      |  ✔️  |  ✔️  |  ✔️  |                    ✔️                   |
| Hair imperfections (blur/lighting effects)                                                      |      |      |      |      |      |      |  ✔️  |  ✔️  |  ✔️  |                    ✔️                   |
| Final Generative Prompt step                                                                    |      |      |      |      |      |      |      |      |  ✔️  |               ✔️ (refined)              |
| Renaming → **Selfie Sections**                                                                  |   –  |   –  |   –  |   –  |   –  |   –  |   –  |   –  |   –  |                    ✔️                   |


---

## 🛠️ Usage  
1. Choose **Selfie** or **Photography** framework depending on the task.  
2. Fill in each section with accurate details (Scene, Clothing, Hair, Expression, etc.).  
3. Merge into a **Final Generative Prompt** for consistent, identity-preserving results.  
4. (Optional) Use alongside **reference images** for stronger accuracy.  

Example (Selfie):  
```text
Generate a realistic handheld selfie of the same person: indoors in a dimly lit public venue with blurred metallic structures, oversized black hoodie (hood up with zipper detail), medium-length dark brown hair slightly messy with strands tucked behind ears, relaxed smile and natural gaze. Close-up handheld selfie at arm’s length, low-up tilt (~10°), centered framing, warm overhead light with soft shadows, natural matte skin with subtle pores and faint freckles, slight motion blur, minor grain, soft edges, candid cozy intimate selfie mood.
```
📌 Why This Matters

- Preserves facial identity and body proportions.
- Produces consistent image quality across variations.
- Prevents common generative issues (plastic skin, incorrect lighting, loss of identity).
- Helps standardize prompt-writing for visual research.

📄 License

This project is licensed under:
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
You are free to share and adapt this work for non-commercial purposes as long as you:
- Provide attribution
- Share under the same license

🤝 Contributing
Suggestions and improvements are welcome!
Open an issue or submit a pull request with refinements, new sections, or additional prompt structures.

🌐 Author

[Gunawan Adi Wijaya]

🔗 LinkedIn: [[Profile](https://www.linkedin.com/in/gnwnadiwjy)]
💻 GitHub: [[Profile](https://github.com/zelunkwn/)]
