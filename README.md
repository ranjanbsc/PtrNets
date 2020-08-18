# PtrNets

This has been forked from https://github.com/vshallc/PtrNets and modified to run in google colab.

Step1: Create dataset for convex hull

!git clone https://github.com/vshallc/PtrNets.git


cd /content/PtrNets/pointer/

!python misc/convex_hull.py ch.pkl.gz


Step2: Run ponternet program like below


!python ptrnets.py ch '/content/PtrNets/pointer/ch.pkl.gz' '/content/PtrNets/pointer/'

#######################################################################################
#######################################################################################
#######################################################################################
# PtrNets
An implementation of Pointer Networks [arXiv:1506.03134](http://arxiv.org/abs/1506.03134)

## Usage
To generate training data

For Convex Hull task:

    >> python misc/convex_hull.py ch.pkl.gz
    
or for TSP task:

    >> python misc/tsp.py tsp.pkl.gz
    
This will generate the training data, add the data path to ptrnets.py (or change the default path in data_util), then start training:

    >> python ptrnets.py
    


## References

* Oriol Vinyals, Meire Fortunato, Navdeep Jaitly,
  "[Pointer Networks](http://arxiv.org/abs/1506.03134)",
  *arXiv:1506.03134 [stat.ML]*.
#######################################################################################
#######################################################################################
#######################################################################################
