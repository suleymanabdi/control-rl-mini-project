# Learning-Based Control of a Nonlinear Dynamical System

---

## 1. Project Motivation

Many real-world control systems operate with imperfect models and uncertain environments. Classical control techniques provide reliable performance when accurate models are available, while learning-based methods offer adaptability but fewer guarantees. This project explores learning-based control applied to a nonlinear system and evaluates its performance relative to classical control methods.

---

## 2. Project Objectives

The objectives of this project are to:

- Stabilize a nonlinear, underactuated system using a learning-based controller  
- Implement a classical controller as a performance baseline  
- Compare performance, robustness, and limitations of both approaches  
- Evaluate the impact of uncertainty and disturbances on controller behavior  
- Develop insight into tradeoffs between model-based and data-driven control  

---

## 3. System Description

### 3.1 Physical System

- **System:** Inverted pendulum on a cart  
- **Degrees of freedom:**  
  - Horizontal cart motion  
  - Pendulum angular motion in a vertical plane  

### 3.2 State Variables

The system state is defined as:

x = [x, x_dot, theta, theta_dot]

where:
- \(x\) is the cart position  
- \(\dot{x}\) is the cart velocity  
- \(\theta\) is the pendulum angle from the upright position  
- \(\dot{\theta}\) is the angular velocity  

### 3.3 Control Input

u ∈ ℝ

The control input is bounded.

---

## 4. Mathematical Model

The system dynamics are nonlinear and continuous-time:

x_dot = f(x, u)

A nominal model is assumed available for baseline control design, while the learning-based controller operates without direct access to the model during execution.

---

## 5. Control Problem Definition

The control problem consists of:

- Stabilizing the pendulum at the upright equilibrium  
- Maintaining bounded cart position  
- Reducing oscillations and excessive control effort  
- Recovering from non-zero initial conditions  
- Operating within actuator limits  

---

## 6. Baseline Controller

A **classical model-based controller** shall be implemented as a baseline reference.

The baseline controller is used to:

- Establish nominal performance  
- Highlight limitations under uncertainty  
- Provide comparison metrics for learning-based control  

---

## 7. Learning-Based Controller

A learning-based controller shall be implemented with the following characteristics:

- Uses measured system states as inputs  
- Outputs control actions directly or indirectly  
- Learns through interaction with the system or simulation  
- Does not rely on online knowledge of system equations  

---

## 8. Optional Hybrid Control

A hybrid approach combining classical and learning-based elements may be implemented.

If included, the hybrid controller must be evaluated independently and compared against both standalone controllers.

---

## 9. Operating Conditions

### 9.1 Nominal Conditions

- Nominal system parameters  
- No disturbances  
- Noise-free measurements  

### 9.2 Non-Nominal Conditions

At least **two** of the following must be considered:

- Parameter uncertainty  
- External disturbances  
- Sensor noise  
- Actuator saturation  
- Increased friction or damping  

---

## 10. Performance Metrics

Controller performance shall be evaluated using:

- Stability (bounded state behavior)  
- Settling time  
- Overshoot  
- Control effort  
- Disturbance recovery time  

All metrics must be applied consistently.

---

## 11. Experimental Evaluation

The project must include:

- Time-domain simulations  
- Identical initial conditions across controllers  
- Quantitative performance comparison  
- Clear presentation of results  

---

## 12. Analysis and Discussion

The final analysis must include:

- Comparison between classical and learning-based controllers  
- Discussion of strengths and weaknesses of each approach  
- Observations on robustness and sensitivity  
- Identification of failure cases  

---

## 13. Deliverables

1. System model description  
2. Controller definitions  
3. Simulation setup  
4. Performance results  
5. Comparative analysis  
6. Final technical report  

---

## 14. Assessment Criteria

The project will be evaluated based on:

- Correctness of implementation  
- Quality of analysis  
- Clarity of results  
- Depth of understanding of control concepts  
- Reproducibility  

---

## 15. Expected Level

This project is suitable for:

- Graduate-level coursework  
- Master’s capstone project  
- Introductory research exposure in control and robotics  
