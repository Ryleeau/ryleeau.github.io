---
layout: essay
type: essay
title: "AI: Learning Reinvented"
# All dates must be YYYY-MM-DD format!
date: 2024-12-14
published: true
labels:
  - Artificial Intelligence
  - Learning
---

<img width="300px" class="rounded float-start pe-4" src="../img/ai.png"> 

## Introduction

AI, or Artificial Intelligence has transformed learning, enriching the student learning experience by providing tools and techniques. These tools and techniques optimize time and bridge the gap between the learning and the working sides of software engineering. In software engineering, AI automates repetitive tasks, in that it provides intelligent analysis that contributes to a software engineer's productivity and creativity. Some AI concepts and tools include machine learning, automated testing, and collaboration tools like Liveshare in vscode. I personally use ChatGPT to enhance my software engineering learning.


## Personal Experience with AI

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

## Impact on Learning and Understanding

## Practical Applications

## Challenges and Opportunities

## Comparative Analysis

## Future Considerations

## Conclusion

Design patterns are the architectural blueprints of software engineering, guiding developers to efficient and usable systems. Just as architects design buildings with structural integrity, developers use design patterns to construct code that is flexible, scalable, and easy to maintain. They bridge the gap between abstract concepts and practical solutions, transforming potential chaos into orderly systems.
