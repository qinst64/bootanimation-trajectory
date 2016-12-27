### bootanimation-trajectory
Analysis of the android 5.0 lollipop bootanimation particle trajectories

---

#### Introduction
A boring stuff I did years ago. The magic bootanimation attracts me: my eyes always lose themselves when trying to catch the magic trajectories of the particles. How can this happen? What is the secret behind?

#### Bootanimation
The `bootanimation.zip` contains a series of `png` images and a `desc.txt` . The images can be extracted from the zip file, which is located in `/system/media/`.

To display the animation, I combined the images into a gif...

![android lollipop bootanimation](bootanimation.gif)

#### Image concatenation
List out all the images...

![bootanimation concatenation 1](concatenation_1.png)

without margin...

![bootanimation concatenation 2](concatenation_2.png)

or even overlap (concatenation from z)...

![bootanimation concatenation 3](concatenation_3.png)

#### Frame by frame analysis

Still, above tricks do not show what I want (last one is close). Some analytical tool is needed to quantify the movement...

![bootanimation concatenation trajectory analysis](trajectory_analysis.png)


Then use matlab to plot the trajectories (with interpolation) ...
![bootanimation concatenation trajectory 1](trajectory_1.png)

Visualization of the trajectories with an additional axis: time...

![bootanimation concatenation trajectory 2](trajectory_2.png)

Code is [here](trajectory.m) (contains particle location data extracted from each frame)

### Conclusion
The above pictures show the results. Em... the trajectories do not seem to be symmetric... 
