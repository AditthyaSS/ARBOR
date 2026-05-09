# ARBOR 🌳🤖

## Adaptive ROS2-Based Behaviour Orchestration for Autonomous Service Robotics

> Autonomous Multi-Agent Service Robot with Adaptive Modular Arbitration (AMA) Framework

![ROS2](https://img.shields.io/badge/ROS2-Humble-blue)
![Platform](https://img.shields.io/badge/Platform-Raspberry%20Pi%205-green)
![Arduino](https://img.shields.io/badge/Microcontroller-Arduino%20Uno-orange)
![Status](https://img.shields.io/badge/Project-Research%20Prototype-purple)
![Domain](https://img.shields.io/badge/Domain-Robotics%20%26%20Autonomous%20Systems-red)

---

# 📌 Overview

ARBOR is a modular ROS2-based autonomous service robotics framework designed to explore adaptive behaviour orchestration in dynamic indoor environments.

Unlike traditional service robots that rely on rigid finite state machines (FSM) or static priority systems, ARBOR introduces an **Adaptive Modular Arbitration (AMA)** framework that allows multiple behaviour agents to dynamically coordinate in real time.

The system combines:

* Autonomous indoor navigation
* Hazard monitoring and obstacle response
* Human interaction modules
* Context-aware arbitration
* Cooperative behaviour blending
* Real-time observability dashboard

ARBOR is built as a practical robotics systems engineering project using:

* Raspberry Pi 5
* Arduino Uno
* ROS2 Humble
* Nav2
* SLAM Toolbox
* OpenCV
* React Dashboard

---

# 🎯 Core Research Idea

The project explores:

> **Adaptive Modular Arbitration (AMA)** for autonomous service robotics.

Instead of a single centralized controller with fixed priorities, ARBOR uses multiple independent behaviour agents that continuously compete and cooperate based on environmental context.

The framework focuses on:

* Context-aware adaptive arbitration
* Cooperative behaviour blending
* Reinforcement-inspired adaptive tuning
* Modular ROS2 architecture
* Embedded observability
* Fault-tolerant operation

---

# 🧠 Adaptive Modular Arbitration (AMA)

The AMA framework is the core innovation of ARBOR.

Each behaviour agent generates:

* a desired action
* a priority bid

The AMA Manager dynamically evaluates these bids using:

* obstacle proximity
* navigation urgency
* human interaction context
* environmental conditions

## Arbitration Formula

```math
Bid_i = BaseBid_i × W_i(C)
```

Where:

* `BaseBid_i` = raw behavioural urgency
* `W_i(C)` = context-aware adaptive weight
* `C` = environmental context vector

---

# ⚙️ Key Features

## 🚗 Autonomous Navigation

* ROS2 Nav2 integration
* Indoor waypoint navigation
* SLAM-based localization
* Dynamic obstacle response

## ⚠️ Hazard Monitoring

* Ultrasonic obstacle sensing
* Real-time hazard detection
* Safety-priority arbitration
* Emergency stop logic

## 🙂 Social Interaction

* OLED eye expressions
* Human-aware behavioural adaptation
* Camera gimbal interaction system
* Interactive robot feedback

## 🧩 Modular Multi-Agent Architecture

* Independent ROS2 behaviour nodes
* Distributed arbitration framework
* Cooperative behaviour blending
* Fault-tolerant node structure

## 📊 Real-Time Dashboard

* Live telemetry monitoring
* Arbitration visualization
* Sensor state monitoring
* ROS2 observability interface

---

# 🏗️ System Architecture

```text
Sensors
   ↓
ROS2 Nodes
   ↓
Behaviour Agents
   ↓
Adaptive Modular Arbitration (AMA)
   ↓
Nav2 / Motion Commands
   ↓
Arduino Control Layer
   ↓
Motor Driver & Actuators
   ↓
Robot Motion
```

---

# 🤖 Behaviour Agents

| Agent                    | Responsibility                              |
| ------------------------ | ------------------------------------------- |
| Navigator Agent          | Autonomous movement and waypoint navigation |
| Hazard Monitoring Agent  | Obstacle detection and safety response      |
| Social Interaction Agent | Human interaction and expressive feedback   |

Each agent:

* runs independently
* publishes behavioural bids
* generates motion intent
* communicates through ROS2 topics

The AMA Manager arbitrates between all active agents.

---

# 🛠️ Hardware Stack

| Component                  | Purpose                    |
| -------------------------- | -------------------------- |
| Raspberry Pi 5             | High-level ROS2 compute    |
| Arduino Uno                | Low-level hardware control |
| Differential Drive Chassis | Robot locomotion           |
| DC Gear Motors             | Motion actuation           |
| Wheel Encoders             | Odometry                   |
| HC-SR04 Sensors            | Obstacle detection         |
| Raspberry Pi Camera        | Vision processing          |
| OLED Displays              | Robot facial interface     |
| Servo Gimbal               | Camera movement            |
| MPU6050 IMU                | Orientation sensing        |
| L298N Motor Driver         | Motor PWM control          |
| Li-Ion Battery Pack        | Power system               |

---

# 💻 Software Stack

| Technology   | Role                    |
| ------------ | ----------------------- |
| ROS2 Humble  | Robotics middleware     |
| Nav2         | Autonomous navigation   |
| SLAM Toolbox | Mapping & localization  |
| OpenCV       | Vision processing       |
| Python       | Agent development       |
| rosbridge    | Dashboard communication |
| React.js     | Observability dashboard |
| RViz2        | Robot visualization     |
| Gazebo       | Simulation environment  |

---

# 📡 ROS2 Node Structure

| Node                | Function               |
| ------------------- | ---------------------- |
| `/navigator_agent`  | Navigation logic       |
| `/hazard_agent`     | Obstacle monitoring    |
| `/social_agent`     | Human interaction      |
| `/ama_manager`      | Arbitration engine     |
| `/dashboard_bridge` | Dashboard telemetry    |
| `/arduino_bridge`   | Hardware communication |

---

# 🔄 Data Flow

```text
Sensors
→ Arduino
→ Raspberry Pi
→ ROS2 Nodes
→ AMA Manager
→ Navigation Decision
→ Arduino
→ Motor Driver
→ Motors
```

---

# 🧪 Planned Experimental Scenarios

* Autonomous waypoint traversal
* Dynamic obstacle avoidance
* Human interaction response
* Arbitration transition analysis
* Fault-tolerant behaviour testing

---

# 📈 Expected Outcomes

* Smooth adaptive behaviour transitions
* Reduced abrupt control switching
* Real-time observability
* Modular scalable robotics framework
* Improved behavioural coordination
* Low-cost autonomous robotics platform

---

# 🔬 Innovation Highlights

## ✅ Context-Aware Adaptive Arbitration

Dynamic bid modulation based on environmental state.

## ✅ Cooperative Behaviour Blending

Multiple agents can cooperate simultaneously instead of hard switching.

## ✅ Reinforcement-Inspired Adaptive Tuning

AMA weights adapt over time using operational feedback.

## ✅ Embedded Observability

Live dashboard monitoring integrated directly into the system architecture.

## ✅ Fault-Tolerant Operation

Graceful degradation when individual behaviour nodes fail.

---

# 🚧 Current Development Status

| Module                        | Status         |
| ----------------------------- | -------------- |
| System Architecture           | ✅ Completed    |
| Hardware Planning             | ✅ Completed    |
| ROS2 Framework Design         | ✅ Completed    |
| AMA Framework Design          | ✅ Completed    |
| Hardware Integration Planning | ✅ Completed    |
| Dashboard Architecture        | ✅ Completed    |
| Physical Robot Build          | 🚧 In Progress |
| ROS2 Implementation           | 🚧 In Progress |
| AMA Integration               | 🚧 In Progress |
| Final Testing                 | ⏳ Planned      |

---

# 📚 Research Foundations

ARBOR is inspired by:

* ROS2 distributed robotics systems
* Behaviour-based robotics
* Hybrid reactive-deliberative architectures
* Multi-agent robotics systems
* Industry 5.0 human-centric robotics
* Embedded observability systems

---

# 🧭 Future Scope

Future extensions may include:

* Conversational AI integration
* Multi-robot coordination
* Semantic mapping
* Voice interaction
* Cloud telemetry synchronization
* Digital twin simulation
* Reinforcement learning policy optimization
* YOLO-based object recognition

---

# 🛡️ System Reliability

ARBOR includes fallback operational modes:

* Teleoperation control
* Emergency manual override
* Pre-mapped navigation mode
* Simplified safe-operation mode

These mechanisms improve deployment reliability in real-world indoor environments.

---

# 👥 Team

## Team 34

* Dayashree S
* Sharan S
* Aditthya SS Varma
* Yashika Bhardwaj
* Nithin Kumar HS

### Institution

Amity University Bengaluru

### Department

ASET

### Faculty Mentor

Dr. Prabin Kumar Jha

---

# 📖 References

Key technologies and concepts used in ARBOR:

* ROS2 Humble
* Nav2 Navigation Stack
* SLAM Toolbox
* OpenCV
* Behaviour-Based Robotics
* Multi-Agent Arbitration Systems
* Industry 5.0 Robotics

---

# ⭐ Project Vision

ARBOR aims to serve as:

* a robotics research platform,
* a ROS2 educational framework,
* and a modular autonomous service robot architecture for future intelligent robotic systems.

---

# 📜 License

This project is currently developed as part of a university innovation and research initiative.

Future open-source licensing details will be added after core implementation completion.

---

# 🌳 ARBOR

> Adaptive coordination for the next generation of modular autonomous robotics.
