# GraphCore

The parameters that I've changed did not give me results that are too different. The following are the conditions that I varied: <br/>

1. Learning rate = 0.03, epoch = 10, batch_size = 8  ---> test data accuracy 96.62%  <br/>

 2. Leaning rate = 0.1, epoch = 10, batch_size = 8  ---> test data accuracy 98.43% <br/>
 
 3. Leaning rate = 0.1, epoch = 5, batch_size = 8 ---> test data accuracy 97.98% <br/>

 4. Leaning rate = 0.0001, epoch = 5, batch_size = 8 ---> test data accuracy  98.61% <br/>

5. Leaning rate = 0.0001, epoch = 5, batch_size = 32 ---> test data accuracy 98.18% <br/>

6. Learning rate = 0.03, epoch = 10, batch_size = 2  ---> test data accuracy 98.35%  <br/>

Based on what I can infer from the code, every time I run the script mnist_poptorch.py, a model is defined and then the parameters are learned.
The reason I bring this up because I was wondering if I am not defining a new model, but only training on top of the last defined model, in which case
my test accuracy would not change much. But based on the code I believe that's not the case. Then, varying these parameter did not change much.
