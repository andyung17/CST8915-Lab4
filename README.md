# CST8915 Lab 4: Development: Introduction to Docker

**Student Name**: Andy Ung <br/>
**Student ID**: 041299387 <br/>
**Course**: CST8915 Full-stack Cloud-native Development <br/>
**Semester**: Fall 2026 <br/>

---

## Demo Video

🎥 [Watch Demo Video]()

## Reflection Questions

1. What are the main differences between a Docker image and a Docker container?

**Image**: Read-only blueprint for construction <br/>
**Container**: Running process isolated on the host machine



2. Explain how Docker's layered architecture improves efficiency.

A dockers layered architecture is building sheets (`Dockerfile`) or stacks out of immutable layers. Since these layers are immutable/read-only, they only add upon the previous allowing for efficient construction. This helps with reusability in which if different projects need the same `OS`, it is able to reuse the core files only once. With this architecture is is able to leveragem, caching to improve efficiency in which modifications to future layers can be combined with pre-existing matching `Dockerfile` to add onto.

3. Why does each container get its own writable layer?

4. What are the benefits of using Docker Compose over running containers individually?

---

## Challenges and Learnings (Optional)

## Acknowledgments
- https://www.geeksforgeeks.org/devops/what-is-docker-layered-file-system/
