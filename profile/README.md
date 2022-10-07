# Solar Wind Cars

Project made on [NASA Space Apps Challenge Prague 2022](https://2022.spaceappschallenge.org/) hackathon. The challenge was to display creatively  data form Parker Solar Probe.

Our team was called Singularity

## What we created

* Unity racing car game
* Website with education content
* Backend that parses data from Parek Solar Probe


```mermaid
sequenceDiagram
    Website->>Unity Game: load Unity IFrame
    Unity Game->>Backend: GET /data
    activate Unity Game
    activate Backend
    Backend->>Solar Probe Data: get sensor data
    Solar Probe Data->>Backend: return sensor data
    Backend->>Backend: parse data
    Backend->>Unity Game: return parsed data
    deactivate Backend
    Unity Game->>Unity Game: load data
    Unity Game->>Unity Game: start race
    deactivate Unity Game   
```

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
