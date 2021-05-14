# Recursive Just-The-Docs

I wanted a recursive just-the-docs menu so I could have more than just 2 or 3 levels in my nav tree so I made it real!

This code is by no means ready to merge with the main just-the-docs repo but it works and is 90% there. I hope that someone takes my code and makes it a little more professional (I am only a 16yo so I don't have the best code lol) and adds it to the official just-the-docs repo.

## How to use the recursive feature
It is important to set the parent variable for each page like before but you dont have to set the grand_parrent variable. instead you set the parents variable. the parents variable is an array with the names of all of the parents/grand parents/great grand parents/etc. Right now you have to list them in order from the parent first and the oldest grand parent last but that will later change as this arrangement means that you have to later reverse the array order in the code.

### Ex:
If I have a page called cameras and this is its location in the tree:
/Boston Dynamics/Robots/Spot/Hardware/Cameras
This is what the file would look like:
```
---
title: Cameras
parents:
  - Hardware
  - Spot
  - Robots
  - Boston Dynamics
parent: Hardware
has_children: true
nav_order: 1
permalink: /boston-dynamics/robots/spot/hardware/cameras
---
```
