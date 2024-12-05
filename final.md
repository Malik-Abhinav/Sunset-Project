# Milestone #7 - Final Delivery  

## Video Walkthrough  
A video walkthrough of our project showcasing the implemented features, system architecture, and deployment process is available at the following link:  
[**Video Walkthrough Link**](https://your-video-link.com)  

---

## General Development  

### 1. What did your team build?  
We built a simplified Discord clone, a web-based communication platform designed for real-time messaging and user interaction. The key features include:  
- **Authentication:** Users can sign up, log in, and log out.  
- **Messaging:** Real-time messaging with multiple channels.  
- **UI/UX Design:** An intuitive and responsive interface.  

---

### 2. Requirements Checklist  
| Feature                | State (Complete/Incomplete) | Notes                          |
|------------------------|-----------------------------|--------------------------------|
| Authentication         | Complete                   | Using Clerk for seamless integration.  
| Real-time Messaging    | Complete                   | Fully functional utilizing Stream.  
| Server and Channel Creation    | Complete                   | Fully functional using APIs, Next.js, and Tailwind CSS
| CI/CD Pipeline         | Complete                   | Tested and operational.  
| Dockerization          | Complete                   | Ready for deployment with Docker.  

All initial requirements were delivered as planned, and our requirements sufficiently captured project details.  

---

### 3. System Architecture  
The system uses a **client-server architecture** with the following components:  
- **Frontend:** Built with Next.js and TypeScript for a dynamic user experience.  
- **Backend:** Node.js server with REST APIs for user and messaging services.  
- **Database:** Clerk and Stream both host and store data related to users and messaging.

---

### 4. Code Reuse  
The project extensively reused shared utility functions, design pattern implementations, and third-party libraries. This streamlined development and reduced redundancy.  

---

### 5. Backlog  
There are no major tasks left in the backlog. The remaining items are minor enhancements and non-essential features.  

---

## CI/CD  

### 1. Testing Strategies  
- **Unit Tests:** Automated with Jest for all core modules.  
- **Integration Tests:** End-to-end tests for key workflows.  
- **Future Improvements:** Increase test coverage earlier in development to minimize debugging overhead.  

---

### 2. Branching Workflow  
Our team followed a **feature-branch workflow**:  
- Each branch underwent code reviews via pull requests.  
- Merging was smooth with minimal conflicts.  

---

### 3. Deployment  
The project is Dockerized with:  
- Dockerfiles for the frontend and backend.  
- A `docker-compose` configuration for multi-container orchestration.  

To deploy:  
1. Clone the repo.  
2. Run `docker-compose up`.  

---

## Reflections  

### 1. Project Management  

---

### 2. Requirements  
The initial requirements were detailed and sufficient. However, we overlooked the time needed for testing and minor UI enhancements.  

---

### 3. Planning Gaps  
Missed accounting for deployment challenges and setting up CI/CD pipelines early.  

---

### 4. Process Management and Observations

---

### 5. IDE and Environment Issues  
We encountered minor issues with differing IDE setups, resolved by agreeing on shared configurations.  

---

### 6. Effort Estimation  
Initial estimations underestimated testing and debugging time. Future estimates will account for these.  

---

### 7. Unique Contribution and Learning
In our project, one of the most unique challenges we faced was integrating the Clerk.io API for authentication. For a long time, it wasn't working correctly, and we kept encountering errors that were difficult to diagnose. After extensive debugging and scouring online forums, we discovered the issue: our system clocks were slightly desynchronized—off by just two seconds.

Since Clerk.io generates authentication keys that are only valid for a few seconds, our keys were expiring before they could be used, making authentication fail every time. This was a big learning moment for us. It taught us that not all issues are logical or syntax-based. Sometimes, the problems lie outside the code, in areas like system settings or environment configurations. This experience emphasized the importance of looking beyond the obvious and reinforced the value of persistence and thorough investigation in problem-solving.

---

### 8. AI's Impact  
The impact of AI in our project was mainly used for debugging. AI helped us understand the error messages and possible causes that pointed us to the correct direction on where to make the changes which resulted in an easier debugging process.

---
