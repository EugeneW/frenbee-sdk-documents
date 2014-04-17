▶ [[Model design specifications]] ▶ Morph animation design tips

---

When you use a Facial Expression Morph in combination, be sure to check the geometry by setting the `Lip_Size` morph value to 1.0 (100%) temporarily.
Care needs to be exercised especially when you superimpose the `Mouth_Laughing` or `Mouth_Surprised` morph that causes the mouth to open wide.
If the geometry around the mouth is disrupted, set a smaller morph value or make other necessary adjustments.

> Do not forget to set the `Lip_Size` morph value back to 0.0 (0%) after checking the geometry, and avoid hitting the animation key.

![morph.png](morph.png)