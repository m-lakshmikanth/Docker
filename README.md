
This repository is my personal deep-dive into Docker. Instead of just running random commands, I’ve broken down the core mechanics of containerization to understand how to build efficient, secure, and production-ready images.

## How it’s organized

I’ve structured this like a hands-on handbook. Each folder focuses on a specific Dockerfile instruction so you can see exactly how they impact the build process.

  * **The Fundamentals**: Examples for `FROM`, `RUN`, `CMD`, and `ENTRYPOINT`—the core of any container.
  * **File Management**: Practical differences between `ADD` and `COPY` for moving data.
  * **Config & Logic**: Using `ENV` and `ARG` to make images dynamic, plus `WORKDIR` and `USER` for better structure and security.
  * **Real-World Setup**: The `Expense_docker/` folder shows how all these individual pieces come together to containerize a full application stack.

## Key Takeaways

  * **Optimization**: Layering instructions correctly to keep image sizes small.
  * **Security**: Moving away from "root" by default using the `USER` instruction.
  * **Execution**: Mastering the nuances of `CMD` vs `ENTRYPOINT` for better container flexibility.

## How to use it

Each folder is standalone. To test an instruction:

1.  **Jump into a folder**: `cd ARG`
2.  **Build it**: `docker build -t test-image .`
3.  **Run it**: `docker run test-image`

-----
