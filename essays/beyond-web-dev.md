---
layout: essay
type: essay
title: "Reflecting on Software Engineering: Beyond Web Development"
date: 2025-05-14
published: true
labels:
  - Agile Project Management
  - Configuration Management
  - Ethics
  - Software Engineering
---
<div style="text-align: center;">
  <img src="../img/software-engin.webp" alt="Software Engineering" style="width: 300px; border-radius: 15px; display: block; margin: 0 auto;">
  <p style="margin-top: 10px;">Source: Gisma</p>
</div>

<hr>

Throughout the development of our final project, DormU, I realized that software engineering is not simply about writing code. It’s about discipline, communication, and conscious decision-making. This course wasn’t just a crash course in Next.js or Prisma, but rather a full exposure to what it means to build scalable, collaborative, and ethical software.

## Agile Project Management
Before this class, project management always felt like an afterthought—something tacked on rather than built in. But implementing **Issue Driven Project Management** (IDPM) within our GitHub board gave the DormU team structure. Breaking tasks into issues and associating them with milestones created a clear path from idea to implementation. It made the overwhelming process of building a platform feel digestible. That said, IDPM also showed its limits when collaboration faltered. At times, we worked in silos, completing our own assigned issues without a full picture of others’ progress. It taught me that Agile isn’t just a checklist; it requires communication. Moving forward, I’d want to incorporate more intentional stand-ups and sync meetings so that issues get done more efficiently.

## Configuration Management: Invisible But Essential
One of the most eye-opening lessons was how critical **Configuration Management** is. At one point, our Prisma schema migrations failed due to version mismatches between local and deployed environments. Even though the code looked fine, Vercel couldn’t connect to the database correctly. The issue wasn’t logic—it was configuration. Version control through Git saved us numerous times, and I now fully appreciate the need for reproducibility. It reminded me of an earlier course where I had to format C code exactly according to strict specs or risk point deductions. It was tedious at the time, but it emphasized the importance of consistency and that habit stuck with me in this class.

```
// ESLint enforced formatting
function sumFor(list: number[]): number {
  let sum = 0;
  for (let i = 0; i < list.length; i++) {
    sum += list[i];
  }
  return sum;
}
```
Using tools like ESLint in VSCode made these rules easier to live with, but more importantly, it helped maintain a standard that all teammates could rely on. This is critical when working across a shared codebase.

## Ethics and the Double-Edged Sword of AI Assistance
When it came to AI-assisted coding, I often found myself walking a fine line. While ChatGPT helped clarify TypeScript quirks and generated snippets for things like ESLint configs or functional patterns, it also sometimes gave me misleading answers, especially when it didn’t understand the structure of my actual app. In one WOD, I asked it to help with an inventory update function for smoothies. This seemed right, but our actual inventory used an array of ingredient objects, not key-value pairs. I only caught the bug after debugging the entire smoothie flow. That experience reminded me that AI can speed things up, but not always accurately, and that understanding the context matters more than just copying code. What’s more concerning is how easy it is to fall into dependency. There were times I knew, deep down, that I could solve a problem if I sat with it longer, but I asked AI anyway. It made me reflect: am I learning, or outsourcing my thinking?

## Design Patterns: Order in the Chaos
In DormU, design patterns became my guideposts. Using the container/presentational pattern helped me separate concerns on the profile page:
```
// app/profile/page.tsx
import BioSection from '@/components/BioSection';
import PostFeed from '@/components/PostFeed';

export default function ProfilePage() {
  return (
    <main>
      <BioSection />
      <PostFeed />
    </main>
  );
}
```
These patterns weren’t just about code cleanliness, allowed our team to iterate faster without stepping on each other’s toes. Similarly, the provider pattern made it easier to pass session data across the app without redundancy. Conclusively, I found that design patterns significantly aided our app scale with clarity and consistency.

## Efficiency with Identity with UI Frameworks and Coding Style
Tools like Bootstrap 5 were a lifesaver. I used to think using frameworks was “cheating” or lazy, but this course helped me reframe that. Just like we buy furniture instead of crafting it from raw wood, using a UI framework lets us build faster and focus on what matters: user experience and logic. Still, I believe in customization. Leaving everything as the default Bootstrap layout feels lazy. But starting with a framework and shaping it to fit your brand? That’s smart engineering. And just like visual style, I learned that coding style is both a personal signature and a professional expectation. Sometimes it’s okay to write messy for yourself. But when working on a team, standardization becomes essential for communication. In that way, your code is your handwriting—but sometimes, you’re writing for others to read.

## Beyond the Stack
Looking back, this course wasn’t just about building a web app, it taught me how to build software responsibly with tools, standards, and awareness. Whether it’s managing schema changes, debating AI usage, or deciding between raw CSS and Bootstrap, every decision we made reflected deeper software engineering values. I now understand that good software isn’t just what it does. It’s how it’s made, how it’s maintained, and how it impacts the people who build and use it. In short, I learned to think like an engineer, not just a coder.
