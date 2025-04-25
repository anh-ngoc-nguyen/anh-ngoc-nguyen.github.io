---
layout: essay
type: essay
title: "The Power of Design Patterns"
# All dates must be YYYY-MM-DD format!
date: 2025-04-24
published: true
labels:
  - Software Engineering
  - Design Patterns
  - Frontend Development
---

<div style="text-align: center;">
  <img src="../img/pattern.jpg" alt="Design Patterns" style="width: 300px; border-radius: 15px; display: block; margin: 0 auto;">
  <p style="margin-top: 10px;">Source: Medium</p>
</div>

<hr>

## Nature’s Blueprint
Many people may not be aware of the similarities, but there are countless everyday objects we see that are designed to reflect patterns found in nature. Engineers and architects alike sometimes use design patterns that mimic wildlife features or behavior in order to solve various issues. In Japan, the first Shinkansen bullet trains were notoriously loud and caused disturbances to the local residents. To combat this, the bullet train was re-modeled after the Kingfisher bird, adopting a long, beak-shaped nose to reduce noise pollution and even save electricity. Although a Kingfisher and a bullet train may use their designs for different purposes, the shared pattern is what helps efficiently improve their individual functionalities.

## The Role of Design Patterns in Software
Rather than solving the same problem over and over, we can tackle it by identifying a common structure and re-using it as a solution. In this way, it serves as a conceptual blueprint or template for future cases and helps maintain consistency throughout projects. Within software engineering, design patterns become essential especially in the context of large-scale development. If everyone in an organization or team follows a shared structure, it helps eliminate confusion around code readability, scalability, and maintenance. Design patterns not only optimize workflow amongst teammates but also serve as a learning tool for beginners to experience good software practice. However, they do come with a double-edged sword, as every pattern can introduce unnecessary complexity or limitations. Not every issue can be solved with a design pattern, so it’s crucial to understand when and where to apply them. When executed correctly, though, they can significantly improve progress.

## Using Patterns to Build 
In developing DormU, a web platform designed for student dormitory networking, I leaned on the power of design patterns to guide the structure and functionality of the application. By separating logic from presentation through the container/presentational pattern, I ensured that our visual components remained clean, reusable, and easy to maintain. For example, the profile page I created in DormU separates responsibilities by handling data and page structure, while visual components like BioSection and PostFeed focus only on how things are displayed.
```
// app/profile/page.tsx
// page.tsx file for Profile page on DormU

import BioSection from '@/components/BioSection';
import PostFeed from '@/components/PostFeed';
…
```
The provider pattern also helped me manage shared data like user sessions across different parts of the app. These patterns weren’t just technical decisions, they acted as anchors in a team environment, enabling collaboration and quicker iterations. I found that embracing design patterns kept our codebase efficient, understandable, and scalable, even as features and complexity grew.

## Patterns That Shape Progress
Just as the Kingfisher-inspired bullet train solved disruptions by adopting nature’s design, software engineers solve recurring challenges by embracing design patterns. These patterns act as bridges that connect technical problems to solutions that improve efficiency, teamwork, and clarity. From visual presentation to data management, the patterns I used in DormU helped streamline development and made the codebase more adaptable to future changes. Recognizing and applying these shared structures not only reflects thoughtful design but also sets the foundation for sustainable growth in any project.
