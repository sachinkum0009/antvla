# AntVLA
VLA designed to navigate Mobile Robots

![AntVLA](docs/media/antvla.png)

## Navigation with VLA

The idea is to implement the VLA which can understand the environment and make decisions to navigate the robot.

## Architecture

```mermaid
graph TD
    subgraph C[AntVLA]
        subgraph E[VLM]
            F[LLM + ViT]
        end
        E --> G[DiT]
    end
    A[Image Token] --> C
    B[Text Token] --> C
    C --> D[Action Token]
```
