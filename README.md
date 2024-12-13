<p align="center" style="font-size:40px;">
<b>PCLA: A framework for testing autonomous agents in CARLA simulator</b>
</p>

<p align="center" style="font-size:20px;">
PCLA (Pretrained CARLA Leaderboard Agent) is a versatile framework that allows you to utilize the autonomous agents from the <a href="https://leaderboard.carla.org/leaderboard/">CARLA Leaderboard</a> independently of its core codebase and put them on your vehicle. With PCLA, you can have with your own CARLA API code and then easily deploy your selected autonomous agents to your vehicles. Additionally, PCLA lets you work with the latest version of CARLA, freeing you from the limitations of using a specific version.
</p>

This repository
was tested on Linux ubuntu 22 and carla 9.15
ValueError: An output representation was chosen that was not trained. : unset DIRECT

## Contents

1. [Setup](#setup)
2. [Pre-Trained Weights](#pre-trained-weights)
3. [Autonomous Agents](#autonomous-agents)
4. [How to Use](#how-to-use)
5. [Sample Code](#sample-code)
6. [Common Mistakes](#common-mistakes)
7. [Citation](#citation)
8. [Acknoledgements](#acknoledgements)

## Setup
Download and install the <a href="https://carla.readthedocs.io/en/latest/">CARLA simulator</a> from the official website. Based on your preference, you can either use quick installation or build from source.</br>
Clone the repository and build the conda environment:
```Shell
git clone https://github.com/MasoudJTehrani/PCLA
cd PCLA
conda env create -f environment.yml
conda activate PCLA
```

## Pre-Trained Weights

Download the pre-trained weights from ????[insert link here] and extract them into the `PCLA/agents/` directory.</br> 
Ensure that each folder of pre-trained weights, is placed directly next to its respective model's folder.

## Autonomous Agents
PCLA includes 9 different autonomous agents and 17 distinct training seeds to choose from.
- **CARLA-garage**
  - Contains 4 different autonomous agents with 3 training seeds for each agent.
    - *lav*, seed 0 to 2.
    - *aim*, seed 0 to 2.
    - *leaderboard*, seed 0 to 2.
    - *longest6*, seed 0 to 2.
  - Repository: [https://github.com/autonomousvision/carla_garage](https://github.com/autonomousvision/carla_garage)
- **Neat**
  - Contains 4 different autonomous agents.
      - *neat*
      - *aimbev*
      - *aim2dsem*
      - *aim2ddepth*
  - Repository: [https://github.com/autonomousvision/neat](https://github.com/autonomousvision/neat)
- **Interfuser**
  - Contains 1 autonomous agent.
     -*interfuser*
  - Repository: [https://github.com/opendilab/InterFuser](https://github.com/opendilab/InterFuser)

## How to Use
