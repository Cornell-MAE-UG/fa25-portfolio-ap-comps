---
layout: project
title: Ball Balancing on Beam
description: LQR Control of Ball on Beam
technologies: [MATLAB]
image: /assets/images/ball-on-beam-post.png
---

For our final project in my Systems Dynamics course (MAE 3260), my group chose to model a **ball on a beam system** and design a controller that can balance the ball before it falls off the beam. Along with it being unique from other systems we studied over the semester, we chose this system due to its physical nature and relative simplicity, which allowed us to make very few modeling simplifications and simulate the physical behavior. 

<div style="clear: both"></div>
<video controls style="width: 250px; margin: 0px 25px 15px 25px vertical-align: top; float: right; margin-right: 0;">
    <source src="{{ 'assets/ball-balancing-on-beam-animation.mp4' | relative_url }}" type="video/mp4">
</video>

{% comment %}
Initial ball position (m): 0.4
Initial ramp angle (rad): 0.3
Initial ball velocity (m/s): 0.1
Initial ramp angular velocity (rad/s): 0
{% endcomment %}

**Key topics of study:**
- Ordinary Differential Equations
- State Space Models
- Feedback Control Law

**My role in the project was modeling the physical system.** This included using concepts from my Dynamics course (MAE 2030), including 2D rigid body motion, to find the equations of motion. I also created the state space model of the system, where I faced one primary challenge: I initially did not know how to make a linear state space model with non-linear equations, so I had to utilize some resources, including my professor's assistance, to do so. 

**My biggest takeaways:** Analyzing a dynamical system from start to finish deepened my understanding of how each component we learned about in class (modeling, state space, feedback control) is applied in context and how they fit together. Additionally, having to do so on our own (as opposed to being given the setup) challenged us to make the decisions and ask important questions: how much do we simplify our model, and how does this affect the rest of the project? is PID the best type of control law for our system?  

**Here is our final report,** which includes modeling the system, designing an LQR controller, and simulating the result:
<iframe src="{{ 'assets/systems-report-pretty.pdf#toolbar=0&navpanes=0' | relative_url }}" width="600" height="750" frameborder="0"></iframe>

