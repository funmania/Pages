# Plan: Remove Medical/Diagnostic Language from Privacy & Terms

## Goal
Remove all language that suggests the app diagnoses, treats, or calculates based on health conditions. The app should appear as a **general nutrition tracking tool**, not a medical system.

---

## Changes for privacy.html

### Line 76
- **Current:** `"Health Information: Activity level, health conditions (e.g., diabetes, IBS, celiac), allergies, pregnancy/breastfeeding status, dietary preferences"`
- **Replace with:** `"Health Information: Activity level, dietary preferences, allergies, and lifestyle factors"`

### Line 102
- **Current:** `"Estimate blood sugar impact based on your health conditions"`
- **Replace with:** `"Estimate carbohydrate and glycemic impact based on general nutritional models and user-provided preferences"`

### Line 113
- **Current:** `"blood sugar estimates and nutrient deficiency warnings"`
- **Replace with:** `"nutritional insights and deficiency indicators"`

### Line 120
- **Current:** `"Health conditions (diabetes, IBS, celiac, etc.)"`
- **Replace with:** `"Dietary preferences and restrictions"`

### Line 132
- **Current:** `"Adjust calculations for specific health conditions (e.g., diabetes)"`
- **Replace with:** `"Adjust general nutritional insights based on user preferences and dietary inputs"`

### New Additions in Section 4 (after line 143 - after "We do NOT:" section)
Add a new box with:
```
<div class="bg-surface border-2 border-tertiary p-6 mb-6">
    <h3 class="text-primary font-bold mb-3">Important Clarifications</h3>
    <ul class="list-disc list-inside text-secondary space-y-2">
        <li>The app does not use health information to diagnose, treat, or manage medical conditions.</li>
        <li>Health-related inputs are used only to customize general nutritional insights and do not result in medical or clinical recommendations.</li>
        <li>This app is not a substitute for professional medical advice, diagnosis, or treatment.</li>
    </ul>
</div>
```

---

## Changes for terms.html

### Line 75
- **Current:** `"Blood sugar estimation for health-conscious users"`
- **Replace with:** `"Nutritional impact estimation for health-conscious users"`

### Line 87
- **Current:** `"Blood sugar estimates are approximations and should not replace glucose monitoring"`
- **Replace with:** `"Nutritional estimates are approximations based on general models and should not replace professional guidance"`

### Line 89
- **Current:** `"especially if you have diabetes, are pregnant, or have other health conditions"`
- **Replace with:** `"especially if you have specific dietary needs or health concerns"`

### Line 227
- **Current:** `"Blood sugar impact estimates"`
- **Replace with:** `"Carbohydrate and glycemic impact estimates"`

### Line 232
- **Current:** `"may not account for individual health conditions, allergies, or medical history"`
- **Replace with:** `"may not account for individual dietary preferences, restrictions, or specific needs"`

---

## Changes for index.html

### Line 84
- **Current:** `"Simultaneous tracking of food intake alongside real-time blood sugar telemetry. Identify correlations instantly."`
- **Replace with:** `"Simultaneous tracking of food intake alongside real-time nutritional analysis. Identify patterns instantly."`

### Line 127
- **Current:** `"glucose data point"`
- **Replace with:** `"nutritional data point"`

---

## Summary of Key Principles Applied

1. **No diagnostic language** - Removed all mentions of "diabetes", "IBS", "celiac", "health conditions"
2. **No medical claims** - Changed "blood sugar" to "carbohydrate/glycemic impact" or "nutritional insights"
3. **General nutrition focus** - Emphasized "nutritional insights" and "general models"
4. **Clear disclaimers** - Added explicit statements that app doesn't diagnose/treat medical conditions
5. **User preferences, not conditions** - Focus on "dietary preferences" instead of "health conditions"

---

## Execution Order

1. privacy.html - 6 changes + 1 new section
2. terms.html - 5 changes
3. index.html - 2 changes

Total: 13 changes + 1 new section addition
