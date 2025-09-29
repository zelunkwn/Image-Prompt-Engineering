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

---

<img width="2379" height="1979" alt="image" src="https://github.com/user-attachments/assets/5d136eb3-b54e-4376-bdfd-e079aae0c71d" />


## 📌 Evolution Table — Non-Pose → Selfie
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

## 📌 Evolution Table — Pose → Photography
| Feature / Section                                                                                     | v1.1 | v1.2 | v1.3 | v1.4 | v1.5 | v1.6 | v1.7 | v1.8 |      v2.0 (Photography)      |
| ----------------------------------------------------------------------------------------------------- | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--------------------------: |
| Basic sections (Scene, Clothing, Hair, Expression, Pose, Camera, Lighting, Skin, Imperfections, Mood) |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |              ✔️              |
| Negative / Avoid rules                                                                                |      |      |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |              ✔️              |
| Selfie flag (optional in Scene & Pose)                                                                |      |      |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  | Integrated under Camera/Pose |
| Expanded Pose details (arm, hand, props)                                                              |      |      |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |  ✔️  |              ✔️              |
| Advanced Camera shot types (close-up → extreme wide, cinematic list)                                  |      |      |      |      |      |      |      |      |              ✔️              |
| Camera motion types (tracking, dolly, crane, handheld, steadicam, drone, POV)                         |      |      |      |      |      |      |      |      |              ✔️              |
| Perspective effects (foreshortening, compression, rack focus)                                         |      |      |      |      |      |      |  ✔️  |  ✔️  |              ✔️              |
| Mood linked to lighting + pose                                                                        |      |      |      |      |      |      |      |  ✔️  |              ✔️              |
| Final Generative Prompt step                                                                          |      |      |      |      |      |      |      |  ✔️  |         ✔️ (refined)         |
| Renaming → **Photography Sections**                                                                   |   –  |   –  |   –  |   –  |   –  |   –  |   –  |   –  |              ✔️              |

---

## 📊 Evolution of Accuracy, Realism & Identity Consistency
🔹 Non-Pose → Selfie
| Version           | Accuracy (following instructions) | Realism (photographic believability) | Identity Consistency (face match w/ refs) | Notes                                                                                   |
| ----------------- | --------------------------------- | ------------------------------------ | ----------------------------------------- | --------------------------------------------------------------------------------------- |
| **v1.1**          | 🟢 Basic                          | 🟡 Medium (simple, lacked detail)    | 🟡 Medium (sometimes drifted)             | Too generic; minimal section control.                                                   |
| **v1.2**          | 🟢 Improved                       | 🟡 Medium                            | 🟡 Medium                                 | Added more detail but still loose.                                                      |
| **v1.3**          | 🟢🟢 High                         | 🟢 High                              | 🟢🟢 Very High                            | ✅ Your best-performing version → strong structure, avoids overlap, preserves identity.  |
| **v1.4–v1.6**     | 🟡 Dropped slightly               | 🟡 Medium                            | 🟡 Medium                                 | More complexity = sometimes over-constrained; accuracy dipped.                          |
| **v1.7–v1.9**     | 🟢 High again                     | 🟢 High                              | 🟢 High                                   | Reintroduced natural imperfections & final generative step → realism up.                |
| **v2.0 (Selfie)** | 🟢🟢 Very High                    | 🟢🟢 Very High                       | 🟢🟢 Very High                            | Balanced structure + flexibility, selfie-specific tuning, explicit gaze/arm = top-tier. |

🔹 Pose → Photography
| Version                | Accuracy       | Realism        | Identity Consistency | Notes                                                                                 |
| ---------------------- | -------------- | -------------- | -------------------- | ------------------------------------------------------------------------------------- |
| **v1.1**               | 🟢 Basic       | 🟡 Medium      | 🟡 Medium            | Simple, lacked pose depth.                                                            |
| **v1.2**               | 🟢 Improved    | 🟡 Medium      | 🟡 Medium            | Cleaner but still generic.                                                            |
| **v1.3**               | 🟢🟢 High      | 🟢 High        | 🟢🟢 Very High       | Added explicit selfie/pose details → much stronger identity consistency.              |
| **v1.4–v1.5**          | 🟡 Medium      | 🟡 Medium      | 🟡 Medium            | More rigid, sometimes less accurate than v1.3.                                        |
| **v1.6**               | 🟢 High        | 🟢 High        | 🟢 High              | Realism boost via imperfections + depth cues.                                         |
| **v1.7–v1.8**          | 🟢🟢 Very High | 🟢🟢 Very High | 🟢 High              | Best realism phase — cinematic, natural flaws, cohesive prompts.                      |
| **v2.0 (Photography)** | 🟢🟢 Very High | 🟢🟢 Very High | 🟢🟢 Very High       | Full cinematic shot grammar (wide shot, POV, dolly, etc.). Most flexible & pro-ready. |

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

[[Gunawan Adi Wijaya]](https://www.instagram.com/gnwnadiwjy)

🔗 LinkedIn: [[Profile](https://www.linkedin.com/in/gnwnadiwjy)]
💻 GitHub: [[Profile](https://github.com/zelunkwn/)]
