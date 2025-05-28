# Gesture Recognition System for SpellLink

## Overview

Gesture-based spellcasting is central to the SpellLink experience. Users will perform swipe patterns or draw shapes mid-air to cast spells. The system must be fast, accurate, and forgiving of minor variance.

## Example Spells & Gestures

| Spell Name | Gesture Pattern | Category |
|------------|------------------|----------|
| Expelliarmus | ↘↖↘ (Zigzag) | Offensive |
| Protego | ⭕ (Circle) | Defensive |
| Stupefy | ➡⬅➡ (Back-forth swipe) | Stunning |
| Reducto | ⬇⬇ (Double downward) | Heavy attack |
| Lumos | 🔼 (Upward swipe) | Utility |

## Recognition Method

- **Motion Sensors + Camera**: Track swipe paths
- **Pattern Matching Algorithm**: Compare to gesture templates
- **Edge Smoothing**: Normalize shaky or fast-drawn gestures
- **On-device ML Model (Optional Advanced Stage)**:
    - Learns from user behavior to improve over time
    - Flags confusing gestures for model retraining

## Accuracy Improvement Plan

- Initial training with top 5 gestures
- User feedback for false positives/negatives
- Optional calibration mode for power users

## Challenges + Mitigations

| Challenge | Mitigation |
|----------|------------|
| Varying hand sizes/speeds | Normalize patterns |
| Lighting/Camera issues | Use IMU data fallback |
| Unclear feedback | Add on-screen glow/trace |
