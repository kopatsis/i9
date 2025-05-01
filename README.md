# i9 Fitness Frontend

**Website:** [i9fitness.com](https://i9fitness.com)  
**Status:** Alpha (development currently paused)  
**Framework:** [SvelteKit](https://kit.svelte.dev/)

This is the frontend for **i9 Fitness**, a dynamic, bodyweight-only training system. Workouts are generated on demand and performed alongside a real-time 3D animated robot trainer.

---

## Features

- 🚀 **Workout Generator**: Request fully personalized workouts by difficulty and time.
- 🏃 **Real-Time Execution**: Follow a 3D robot that performs the entire workout in sync.
- 🔁 **Structured Routine**:
  - Dynamic warmup (mobility-focused)
  - 9 bodyweight workout intervals
  - Static cooldown stretches
- 📈 **Feedback System**: Report workout difficulty to influence future recommendations.
- 📚 **Exercise & Stretch Library**: Browse form guides and workout elements.
- 📆 **Workout History**: View all completed workouts.

---

## Project Structure

- **Workout Request & Preview**: Users select difficulty/time and preview robot-rendered script.
- **Workout Playback**: Robot animates full workout routine based on generated JSON script.
- **Post-Workout Feedback**: Submitted to backend to tune individual difficulty and global AI.
- **Navigation**: Full support for browsing workout history and movement library.

---

## Related Services

This frontend interacts with several backend services in the i9 ecosystem:

- [`i9-backend`](https://github.com/kopatsis/i9-backend): Workout generation, CRUD, feedback, and admin (Go / Gin / MongoDB / bbolt)
- [`i9positions`](https://github.com/kopatsis/i9positions): Generates timed movement scripts for 3D robot (Go / Gin / MongoDB / bbolt)
- [`i9payments`](https://github.com/kopatsis/i9payments): Stripe-backed payment system (Go / Gin / MongoDB)

---

## Development

```bash
git clone https://github.com/kopatsis/i9frontend.git
cd i9frontend
pnpm install
pnpm dev
