---
title: "Set custom animation"
component: "Tab"
description: "This example demonstrates how to set custom animation for both previous and next actions on Essential JS 2 Tab component when the tab select."
---

# Set custom animation

Tab supports custom animations for both previous and next actions from the provided animation option of `Animation` library. The animation property also allows you to set easing, duration, and various other effects.

Default animation is given as `SlideLeftIn` for previous tab animation and `SlideRightIn` for next tab animation. You can also disable the animation by setting the animation effect as none.

The sample demonstrates some types of animation that suits Tab. You can check all the animation effects here.

{% aspTab template="tab/animation", sourceFiles="styles.cs" %}

{% endaspTab %}

Output be like the below.

![Custom Animation](../images/animation.PNG)