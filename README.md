# Udacity Deep Reinforcement Learning Nano Degree - Navigation project
This is the submission for the navigation project in Udacity Deep Reinforcement Learning Nano Degree.

# The Environment
For this project, an agent will be trained to collect bananas in a large, square world.

![](Resource/banana.gif)

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

- 0 - move forward.
- 1 - move backward.
- 2 - turn left.
- 3 - turn right.

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

Note: The project environment is similar to, but not identical to the Banana Collector environment on the Unity ML-Agents GitHub page.

# Getting started
**Step 1: Clone the DRLND Repository**  
Please follow the [instructions in the DRLND GitHub repository](https://github.com/udacity/deep-reinforcement-learning#dependencies) to set up your Python environment. These instructions can be found in README.md at the root of the repository. By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.

(For Windows users) The ML-Agents toolkit supports Windows 10. While it might be possible to run the ML-Agents toolkit using other versions of Windows, it has not been tested on other versions. Furthermore, the ML-Agents toolkit has not been tested on a Windows VM such as Bootcamp or Parallels.

**Step 2: Download the Unity Environment**  
Please download and extract the **Banana** application in the current project from one of the links below. You only need to download the environment that matches your operating system:

Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)

Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)

Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)

Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)


**Step 3: Run the notebook for this project inside drlnd environment**  
> jupyter notebook Navigation.ipynb	

**Step 4: Change the path of banana application**  
Please change the path to the banana application based on the location of the application in the following command:
> env = UnityEnvironment(file_name="path/to/your/banana")

**Step 5: Execution**  
The first three sections of the notebook belong to the original task of Udacity to play and try the banana environment. **So, if you want to train the agent or test the agent with my DQN implementation, please jump to section 4.**

The section four contains three cells:
- The first cell is for loading modules and the banana environment.
- The second cell is for training the agent with DQN.
- The third cell is for testing the agent with trained network. The network weights are loaded from 'checkpoint.pth' file.

If you need to only test the agent with trained model, please skip the training cell and execture the other two. In other case, please execute all three available cells in the section 4.

# Report
The implemented method for the training of the agent is explained in the [report](REPORT.md).

<sub><sub>This readme is adapted from Udacity Deep RL Nano Degree course.<sub><sub>

