---
layout: essay
type: essay
title: "Design Pattern Architect"
# All dates must be YYYY-MM-DD format!
date: 2024-12-04
published: true
labels:
  - Design Patterns
  - Problem Solving
  - Software Development
---

<img width="300px" class="rounded float-start pe-4" src="../img/man-are-working-as-architecture-construction-company_81761-404.png"> 

## Having an Architect

Imagine being tasked with building a house. Growing up as a daughter of a carpenter, I've watched and helped with the building of around 10 houses. The foundation must be level and sturdy, the plumbing and water ways functional and efficient, and the layout optimized for accessibility. Without guidance, there might be a leaky roof or creaky floors. This is where being and achitect and having a blueprint comes in handy: proven templates for solving common design problems. In the realm of software development, design patterns are the blueprints.

Design patterns provide structured solutions to recurring issues in software design. These are not lines of code to be copied and pasted, but rather conceptual frameworks that developers can use to adapt to their needs. Like the idea of a house floor plan, this allows for software to be flexible, scalable, and easy to maintain. 

## Being the Architect

In one of my classes a year ago, I was tasked with creating a simple, centralized logging system that all parts of the application could access. I chose to implement the Singleton pattern where one instance of the logger exists across the application. 

```
class Logger:
  _instance = None

  def new(cls,*args,**kwargs):
    if not cls._instance:
      cls._instance=super(Logger,cls).new(cls,*args,**kwargs)
    return cls._instance

  def log(self,message):
    print(f"[LOG]: {message}")

logger1 = Logger()
logger2 = Logger()

print(logger1 is logger2) #should output True
```

This system is so organized and predictable and even better, easier to read.

## Conclusion

Design patterns are the architectural blueprints of software engineering, guiding developers to efficient and usable systems. Just as architects design buildings with structural integrity, developers use design patterns to construct code that is flexible, scalable, and easy to maintain. They bridge the gap between abstract concepts and practical solutions, transforming potential chaos into orderly systems.
