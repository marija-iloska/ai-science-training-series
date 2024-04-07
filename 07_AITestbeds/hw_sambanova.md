# SAMBANOVA

The homework asked us to rerun the premade example by changing the ntasks, which I found in the BertLarge.sh file.
The way the example was setup was so that the training log ouput files would store in the home directory in a folder BertLarge/hf_output/. 
To rerun I needed to move and rename since otherwise it would overwrite files or not run as these ouputs already exist. <br/>

## Comments

Default ntasks 16 <br/>

My first change ntasks 8 <br/>
My second change ntasks 4 <br/>

For all three sitations my traninig loss got to about 8-9, and the learning rate fluctuates around $10^{-6}$. My impression is that the performance doesn't change, however, what does change is how
long it takes to run. A node can do 8 tasks at a time so setting 16 and 8 would be the same, but setting 4 we get less training samples in one second. <br/>

ntasks 16 <br/>
'final_loss': 8.308636665344238, 'training_samples_per_second': 2293.967741560586 <br/>

ntasks 8 <br/>
'final_loss': 8.30873966217041, 'training_samples_per_second': 2293.073659982928 <br/>

ntasks 4 <br/>
'final_loss': 8.350452423095703, 'training_samples_per_second': 1164.2316062943025 <br/>

