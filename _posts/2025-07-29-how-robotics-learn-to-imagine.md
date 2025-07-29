---
layout: post
title: "How Robotics Learn to Imagine: World Models and Embodied AI"
comments: true
author: Aadarsh Ram + Krish Yadav
excerpt_separator: <!--more-->
---
It’s a rainy evening. You’re cycling home when a ball rolls across the road. Instinctively, you slow down. You haven’t seen the child yet, but you already know one is coming.  
Congratulations — you’ve just simulated the future in your head. Now imagine a robot in your place. Would it have stopped in time?
<!--more-->

# How Robotics Learn to Imagine  
## World Models and Embodied AI  

---

## 1. Introduction: Can Robots Daydream?

It’s a rainy evening. You’re cycling home when a ball rolls across the road. Instinctively, you slow down. You haven’t seen the child yet, but you already know one is coming.  
Congratulations — you’ve just simulated the future in your head. Now imagine a robot in your place. Would it have stopped in time?

Robots today can lift, sort, and navigate. But pausing to **predict**? That’s beyond their reactive control systems. In this piece, we explore **Embodied AI** and **World Models**, two ideas that could bring robots closer to human-like foresight.

---

## 2. Embodied AI: When Thinking Requires Doing

Embodied AI grounds intelligence in real-world interaction.  
Unlike traditional models trained only on data, these agents learn by **seeing, moving, and adapting** in their environment — like a warehouse robot planning, gripping, and avoiding obstacles in real time.

Not all learning needs real-world trial. Simulators like **MuJoCo** or **Isaac Gym** enable virtual practice.  
Embodied AI is like teaching a toddler to walk — by letting them walk.

---

## 3. Embodied AI in the Real World

**Boston Dynamics’ Atlas and Spot** exemplify embodied intelligence:

<div style="display: flex; gap: 10px;">
  <img src="/assets/images/blog/atlas.jpg" alt="Atlas by Boston Dynamics" width="48%">
  <img src="/assets/images/blog/spot.jpg" alt="Spot by Boston Dynamics" width="48%">
</div>

- *Atlas*: Parkour and dynamic traversal  
- *Spot*: Autonomous navigation, door opening, inspection tasks

These are not hardcoded behaviors. They emerge from **learned motor control**, **feedback**, and **motion planning**.

Other systems, like mobile manipulators, mix perception, planning, and control to perform complex tasks like sorting and relocating items in warehouses.

---

## 4. From Doing to Dreaming: Why Robots Need a Mind’s Eye

Embodied AI helps agents learn from interaction. But what if exploring is too costly or dangerous?

Enter **World Models** — enabling robots to imagine consequences **before acting**.

---

## 5. World Models: Building a Robot’s Imagination

Imagine a coffee mug on a tilted table. You *predict* it will slide — that’s a mental simulation.

World Models enable machines to simulate similar outcomes:
- Build compact **latent representations** of the environment
- Predict effects of actions internally  
- Plan safer, smarter actions using internal “mental rehearsals”

This allows for counterfactual reasoning, planning, and adaptability in new environments.

---

## 6. The Architecture Behind the Imagination

Inspired by Ha and Schmidhuber’s 2018 *World Models* paper:

![World Model Architecture](/assets/images/blog/world-model-architecture.png)

1. **Visual Encoder (V)** – Compresses inputs into latent space  
2. **Memory Model (M)** – Predicts future latent states using RNNs/RSSMs  
3. **Controller (C)** – Plans optimal actions from predicted rollouts  

This enables internal trial-and-error — **learning in imagination, not reality**.

---

## 7. Why This Changes the Game

World Models let robots:

- Simulate thousands of trajectories quickly  
- Avoid crashing during training  
- Generalize to unfamiliar scenarios  
- Make informed, grounded decisions

> *“It’s like a robot building a mini Bollywood studio in its head and filming futures before acting.”*

Systems like **DreamerV2** showcase how robots can learn motor skills entirely in imagination.

![DreamerV2 in Simulation](/assets/images/blog/dreamerv2.png)

---

## 8. Why Does It Matter to Us?

### Limitations:

#### 1. Prediction Drift
![Prediction Drift](/assets/images/blog/prediction-drift.png)  
Small model errors accumulate, leading to hallucinated futures.

#### 2. Sim-to-Real Gap
![Sim to Real](/assets/images/blog/sim-to-real.jpg)  
Simulators are neat. Real life is unpredictable.

#### 3. Latent Compression
![Latent Space Limitation](/assets/images/blog/latent-limitations.png)  
Fine details often lost in the abstraction process.

---

## 9. Where We're Headed

Despite challenges, research is progressing:

- **Transformers** for long-horizon predictions  
  ![Transformers for World Models](/assets/images/blog/transformer-worldmodel.png)

- **3D-aware imagination** using NeRFs and Gaussian Splatting  
  ![3D-aware Imagination](/assets/images/blog/nerf-robot.png)

- **Curiosity-driven exploration**  
  ![Curious Robot Simulation](/assets/images/blog/curious-robot.png)

- **Language-guided simulation**  
  ![Language-Driven Planning](/assets/images/blog/language-guided.png)

- **Hierarchical planning models**  
  ![Hierarchical Planning](/assets/images/blog/hierarchical.png)

---

## 10. From Dreams to Decisions

World models give robots a **mental workspace** — to simulate, evaluate, and act.  
The future lies in tighter integration between perception, simulation, and control — thinking before moving.

---

## 11. Conclusion

Back to that rainy road.

The human rider slowed down due to an internal simulation. That’s the vision for robots too:  
Not just reacting, but imagining — and **planning intelligently**.

**Embodied AI** connects agents to the physical world.  
**World Models** give them foresight.  
Together, they enable systems that can learn, adapt, and work **alongside humans**, meaningfully.

---


