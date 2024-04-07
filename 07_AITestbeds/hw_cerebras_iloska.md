# CEREBRAS


The homework asked us to rerun the premade example for different batch sizes, specifically 2048, and 512, with the default example being set to 1024.

## For 2048:
Processed 2048000 sample(s) in 304.240142671 seconds. <br/>
Step=100, Loss=9.48438, Rate=6858.71 samples/sec, GlobalRate=6858.72 samples/sec <br/>
Step=200, Loss=8.48438, Rate=6792.56 samples/sec, GlobalRate=6803.14 samples/sec <br/>
Step=300, Loss=7.77344, Rate=6730.20 samples/sec, GlobalRate=6764.53 samples/sec <br/>
Step=400, Loss=7.64062, Rate=6684.74 samples/sec, GlobalRate=6736.67 samples/sec <br/>
Step=500, Loss=7.37500, Rate=6720.11 samples/sec, GlobalRate=6738.07 samples/sec <br/>
Step=600, Loss=7.42188, Rate=6739.74 samples/sec, GlobalRate=6740.53 samples/sec <br/>
Step=700, Loss=7.25000, Rate=6730.38 samples/sec, GlobalRate=6738.18 samples/sec <br/>
Step=800, Loss=7.12500, Rate=6725.75 samples/sec, GlobalRate=6736.24 samples/sec <br/>
Step=900, Loss=7.25000, Rate=6721.37 samples/sec, GlobalRate=6734.26 samples/sec <br/> 
Step=1000, Loss=7.14844, Rate=6712.77 samples/sec, GlobalRate=6731.53 samples/sec <br/>


## For 1024: <br/>

Processed 1024000 sample(s) in 210.627485242 seconds. <br/>
Step=100, Loss=9.48438, Rate=4930.28 samples/sec, GlobalRate=4930.29 samples/sec <br/>
Step=200, Loss=8.35938, Rate=4897.52 samples/sec, GlobalRate=4902.83 samples/sec <br/>
Step=300, Loss=7.91406, Rate=4877.93 samples/sec, GlobalRate=4890.11 samples/sec <br/>
Step=400, Loss=7.54688, Rate=4852.26 samples/sec, GlobalRate=4876.25 samples/sec <br/>
Step=500, Loss=7.46875, Rate=4841.61 samples/sec, GlobalRate=4867.85 samples/sec <br/>
Step=600, Loss=7.39844, Rate=4850.36 samples/sec, GlobalRate=4865.90 samples/sec <br/>
Step=700, Loss=7.35156, Rate=4848.06 samples/sec, GlobalRate=4863.12 samples/sec <br/>
Step=800, Loss=7.25000, Rate=4855.92 samples/sec, GlobalRate=4862.88 samples/sec <br/>
Step=900, Loss=7.21094, Rate=4867.52 samples/sec, GlobalRate=4864.25 samples/sec <br/>
Step=1000, Loss=7.07812, Rate=4850.11 samples/sec, GlobalRate=4861.66 samples/sec <br/>


## For 512: <br/>
RuntimeError: Initial global step 1000 already exceeds max step 1000. <br/>

I am not sure if we needed to modify something else, but my code raises this error for batch size of 512. Both the 1024 and 2048 have a similar loss, even though the 1024 processed half the number of samples.
