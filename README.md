# Team Stem - integral-force

### Team Members:
- **Prince Achoja**  
  Email: princejoseph.pj@yahoo.com
  
- **Abdulsalam Mohammed**  
  Email: ammuftau74@gmail.com
  
- **Abdulrahman abdulsalam**  
  Email: abdulsalamamtech@gmail.com

---

## Project Overview

Project Overview
Integral Force is an AI-powered, gamified learning platform designed to provide learners with the freedom to explore various subjects at their own pace. The platform offers a dynamic, self-directed learning experience with engaging educational content stored securely on the Internet Computer (IC), eliminating reliance on external web resources. Through the use of gamified quizzes and a competitive leaderboard system, Integral Force makes learning more interactive, motivating, and fun. Whether you're a beginner exploring new subjects or an expert seeking advanced knowledge, Integral Force offers tailored, AI-driven learning paths to help you achieve your educational goals.

###Key Features
1. Flexible Learning Experience

Learners can choose from a wide range of subjects and decide when and what to study based on their interests and goals.
Content is stored on the Internet Computer, ensuring reliable, scalable, and secure access to all materials.
Gamified Quizzes

2. Interactive quizzes designed as mini-games to keep learners engaged.
Earn points, badges, and achievements by completing quizzes and challenges.
Timed quizzes and streak bonuses to motivate consistent learning.
Leaderboard System

3. Global and subject-specific leaderboards that encourage healthy competition.
Weekly and monthly rankings to recognize top learners and provide new opportunities for everyone to compete.
Team-based leaderboards for collaborative learning experiences.
AI-Powered Personalization

4. AI provides personalized learning recommendations based on learner progress and preferences.
Immediate feedback on quizzes to guide learners on areas for improvement.
Customized learning paths to suit individual learning styles and needs.
Progress Tracking and Rewards

5. Learners can track their progress through levels, badges, and certificates.
Personalized progress reports provide insights into achievements and areas for growth.
Earn rewards like exclusive content or recognition on the leaderboard for reaching learning milestones.


---

### Problem Statements & Solutions
Problem 1: Lack of Learner Autonomy and Flexibility
Many online learning platforms require learners to follow a rigid course structure, leaving little room for flexibility in what or when to learn. This can lead to disengagement and low motivation among learners who want to explore subjects at their own pace.

Solution:
Integral Force allows learners to choose their own learning path by offering a variety of subjects they can explore at their own pace. Whether a learner wants to start with beginner material or dive into advanced topics, they can make that decision freely. The AI further supports personalized learning by suggesting subjects or areas for improvement based on individual progress.

Problem 2: Lack of Engagement and Motivation in Learning
Many educational platforms rely solely on passive consumption of content, leading to reduced engagement over time. Learners may feel isolated or demotivated due to the absence of interactive elements or a sense of accomplishment.

Solution:
Integral Force integrates gamification to make learning enjoyable and competitive. Through gamified quizzes, time-based challenges, and a comprehensive leaderboard system, learners are constantly motivated to improve and compete with their peers. They can earn points, badges, and rewards that keep them engaged and striving for excellence.

Problem 3: Difficulty in Tracking Progress and Achievements
Learners often struggle to track their learning progress and achievements, which can lead to frustration and reduced commitment to long-term learning goals.

Solution:
Integral Force offers a detailed progress tracking system where learners can monitor their achievements, badges, points, and quiz performance. AI-generated progress reports give them actionable insights into their strengths and areas needing improvement, ensuring a structured and fulfilling learning experience. Leaderboards and badges also offer recognition and motivation for learners to stay consistent.

Problem 4: Dependence on External Resources for Content
Many platforms pull content from third-party sources, which can lead to inconsistencies in the availability, quality, and security of learning materials.

Solution:
All content on Integral Force is stored securely on the Internet Computer (IC), ensuring learners have reliable and seamless access to all educational resources. By hosting all learning materials internally, we eliminate the risk of broken links, slow loading times, or external dependencies.
---

## Technology Stack
- *Frontend:* React.js
- *Backend:* Motoko
- *Database/STRUCTURE:* Hashmap
- *Storage:* Internet Computer (IC) for content storage

----
## Usage Instructions

1. Register or log in to the platform.
2. Choose a subject from the dashboard.
3. Complete the quizzes to earn points and badges.
4. Track your progress through your profile.
5. Compete on the leaderboard with other learners in real-time.


## Contact For support or inquiries, please contact us at princejoseph.pj@yahoo.com

--- 



Welcome to our new `integral-force` project and to the Internet Computer development community.  


To get started, you might want to explore the project directory structure and the default configuration file. Working with this project in your development environment will not affect any production deployment or identity tokens.

To learn more before you start working with `integral-force`, see the following documentation available online:

- [Quick Start](https://internetcomputer.org/docs/current/developer-docs/setup/deploy-locally)
- [SDK Developer Tools](https://internetcomputer.org/docs/current/developer-docs/setup/install)
- [Motoko Programming Language Guide](https://internetcomputer.org/docs/current/motoko/main/motoko)
- [Motoko Language Quick Reference](https://internetcomputer.org/docs/current/motoko/main/language-manual)

If you want to start working on your project right away, you might want to try the following commands:

```bash
cd integral-force/
dfx help
dfx canister --help
```

## Running the project locally

If you want to test your project locally, you can use the following commands:

```bash
# Starts the replica, running in the background
dfx start --background

# Deploys your canisters to the replica and generates your candid interface
dfx deploy
```

Once the job completes, your application will be available at `http://localhost:4943?canisterId={asset_canister_id}`.

If you have made changes to your backend canister, you can generate a new candid interface with

```bash
npm run generate
```

at any time. This is recommended before starting the frontend development server, and will be run automatically any time you run `dfx deploy`.

If you are making frontend changes, you can start a development server with

```bash
npm start
```

Which will start a server at `http://localhost:8080`, proxying API requests to the replica at port 4943.

### Note on frontend environment variables

If you are hosting frontend code somewhere without using DFX, you may need to make one of the following adjustments to ensure your project does not fetch the root key in production:

- set`DFX_NETWORK` to `ic` if you are using Webpack
- use your own preferred method to replace `process.env.DFX_NETWORK` in the autogenerated declarations
  - Setting `canisters -> {asset_canister_id} -> declarations -> env_override to a string` in `dfx.json` will replace `process.env.DFX_NETWORK` with the string in the autogenerated declarations
- Write your own `createActor` constructor
