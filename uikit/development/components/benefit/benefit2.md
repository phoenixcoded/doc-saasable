---
description: >-
  The Benefit2 component displays a section with a background image, a heading,
  and multiple counter blocks with numerical values and descriptions, adjusting
  layout based on screen size.
---

# Benefit2

{% hint style="info" %}
All available props for the Benefit2 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Benefit section.
{% endhint %}

**Component path**: `src/blocks/benefit/Benefit2.tsx`

**Component usage path:**  `src/app/blocks/benefit/benefit2/page.tsx`

**Preview link:** [https://www.saasable.io/blocks/benefit/benefit2](https://www.saasable.io/blocks/benefit/benefit2)

## Props Details

| Prop Name	      | Type                | Description                                                                                                                                                                                                              | Displayed as                                                                                                                            |
| --------------- | ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| **heading**     | `string`            | Main title of the benefit section.                                                                                                                                                                                       | `"Our Key Benefits"`                                                                                                                    |
| **bgImage**     | `string` (optional) | URL or path for the background image.                                                                                                                                                                                    | `"/images/background.jpg"`                                                                                                              |
| **blockDetail** | Array of objects    | <p>Details for each counter block. Each object includes:<br>- <code>counter</code>: <code>number</code><br>- <code>caption</code>: <code>string</code><br>- <code>defaultUnit</code>: <code>string</code> (optional)</p> | `[ { counter: 150, caption: "Clients", defaultUnit: "k" }, { counter: 75, caption: "Projects" }, { counter: 100, caption: "Awards" } ]` |
