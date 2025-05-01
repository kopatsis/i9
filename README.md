# i9 Fitness

[i9fitness.com](https://i9fitness.com) — A fully dynamic, bodyweight-only training system built for personalized progression, intelligent workout generation, and immersive presentation.

## Overview

i9 Fitness generates custom workouts on demand based on length and difficulty, combining curated movement logic with a real-time visual execution system. It blends adaptive training with 3D-animated guidance, providing a focused experience with zero fluff.

Each workout includes:

- **Dynamic warm-up** — Light mobility to prime the body
- **Main workout** — 9 escalating bodyweight intervals tuned to the user's level
- **Cooldown** — Static stretches to restore balance post-session

The system continuously adapts via user feedback, leveling the user’s account while contributing anonymized insight to global difficulty tuning.

## Repos

### [Frontend](https://github.com/kopatsis/i9frontend)
SvelteKit app. Delivers the full user experience: generating and previewing workouts, viewing past sessions, exploring the movement library, and performing workouts alongside a 3D-rendered robot avatar executing every rep in sync.

### [Backend](https://github.com/kopatsis/i9-backend)
Go (Gin) + MongoDB + bbolt. Handles all logic around workout generation, account management, workout history, feedback processing, and system configuration.

### [Positions Microservice](https://github.com/kopatsis/i9positions)
Generates frame-accurate motion "scripts" for the robot avatar. Converts the abstract workout into exact timed poses that the frontend uses for real-time rendering. Also handles animation scripts for previews and the exercise library.

### [Payments Microservice](https://github.com/kopatsis/i9payments)
Stripe-backed billing layer. Manages membership plans and payments. Go (Gin) + MongoDB + Stripe.

## State

The frontend is currently in alpha. Development is paused but will resume shortly.

This repo serves as the canonical index for the i9 system architecture and component ownership.

---

i9 is built to make bodyweight training intelligent, adaptive, and impossible to outgrow.
