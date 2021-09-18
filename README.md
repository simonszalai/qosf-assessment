# QOSF Mentorship Assesment Task

This is my submission for the Quantum Open Source Foundation's Mentorship Program Cohort 4. The task was to train
a variational quantum circuit that produces certain quantum states given some input states. I choose PennyLane to 
solve the task. I created a layered architecture, each layer having parameterized X,Y and Z rotations on each 
qubit, then CNOT gates in a chain pattern connecting each qubit with the next one. In the final solution, this layer
was applied 32 times. This resulted in a very deep circuit, which would be problematic in a real, noisy quantum 
device, but for the sake of this task, it ensured that the network trained quite fast. On the end, I visualized the
results, and also tried what would happen in I supplied states to the network that were not used for training.

### To run the code in DeepNote
I used DeepNote to work on this project. You can simply visit [this](https://deepnote.com/project/QOSF-Assessment-Final-kNSNHBs-TJucUP5FITfVkg/%2Fnotebook.ipynb) link to access the notebook online.

### To run the code locally
1. Clone this repository
2. Install dependencies
```
pip install -r requirements.txt
```
3. Start Jupyter Notebook `jupyter notebook`, then open `notebook.ipynb`