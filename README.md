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

Containers are isolated processes of each apps components, meanwhile an image is a package that includes all the necessary files to run in the container. A container can be started, stopped, restarted and destroyed, meanwhile an image cannot be altered after being made. Images are read-only and if modifications are needed, a new image needs to be created.

2. Explain how Docker's layered architecture improves efficiency.

A dockers layered architecture is building sheets (`Dockerfile`) or stacks out of immutable layers. Since these layers are immutable/read-only, they only add upon the previous allowing for efficient construction. This helps with reusability in which if different projects need the same `OS`, it is able to reuse the core files only once. With this architecture is is able to leveragem, caching to improve efficiency in which modifications to future layers can be combined with pre-existing matching `Dockerfile` to add onto.

3. Why does each container get its own writable layer?

Each container gets its own writable layer as it records the changes in the filesystem at runtime. Without seperate writable layers, two containers would have conflicts with eachother. The writable layer is meant to be thrown away and stores data along the lines of: logs, cache files, session data, etc. It is important to note that when the container gets stopped or deleted, writtable layer is discarded.

4. What are the benefits of using Docker Compose over running containers individually?



---

## Challenges and Learnings (Optional)

## Acknowledgments
- https://www.geeksforgeeks.org/devops/what-is-docker-layered-file-system/
- https://docs.docker.com/get-started/docker-concepts/the-basics/what-is-an-image/