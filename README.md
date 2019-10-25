# Banana-Navigator

For this project, i trained an agent to navigate (and collect bananas!) in a large, square world.
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

0 - move forward.
1 - move backward.
2 - turn left.
3 - turn right.

Solution : The agent should get more than 13.0 for 100 consecutive episodes.

## Getting Started

### Download the Unity Environment

For this project, you will not need to install Unity - this is because we have already built the environment for you, and you can download it from one of the links below. You need only select the environment that matches your operating system:

Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

Then, place the file in the folder in the Banana-Navigation GitHub repository, and unzip (or decompress) the file.

### Output

<img src="/banana.gif" width= 500 px/>

### Instructions

 1. Download the project materials from my GitHub repository. You can download the repository with
  ```
  git clone https://github.com/vickipedia6/Banana-Navigator.git
  ```
 2. Download anaconda or miniconda based on the instructions in the [Anaconda documentation](https://docs.anaconda.com).
 
 3. Create a new conda environment:
  ```
  conda create --name deep-learning python=3
  ```
 4. Enter your new environment:
  * Mac/Linux: >> ``` source activate deep-learning ```
  * Windows: >>  ```activate deep-learning ```
  
 5. Ensure you have numpy, matplotlib, pandas, and jupyter notebook installed by doing the following:
  ```
  conda install numpy matplotlib pandas jupyter notebook
  ```
 6. Run the following to open up the notebook server:
  ```
  jupyter notebook navigation.ipynb
  ```
 7. Execute all the cells in the code
 
### Project results

* The agent achieved 13.04 within 384 episodes which is pretty quick as the expected outstanding episodes was 1800.

<img src="/Avg score.png" width= 700 px/>


<img src="/graph.png" width= 500 px/>


## Built With

* Python 3

## License

This project is licensed under the MIT License - see the [LICENSE.md](License.md) file for details

## Acknowledgments

* The data comes from the Udacity.
