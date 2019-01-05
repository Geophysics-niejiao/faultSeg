
# FaultSeg: using synthetic datasets to train an end-to-end CNN for 3D fault segmentation

**This is a [Keras](https://keras.io/) version of FaultSeg implemented by [Xinming Wu](http://www.jsg.utexas.edu/wu/) for 3D fault segmentation**

As described in **FaultSeg: using synthetic datasets to train an end-to-end CNN for 3D fault segmentation** by [Xinming Wu](http://www.jsg.utexas.edu/wu/)<sup>1</sup>, 
[Luming Liang](https://sites.google.com/site/lumingliangshomepage/)<sup>2</sup>, 
[Yunzhi Shi](https://scholar.google.com/citations?user=t9dQMgIAAAAJ&hl=en)<sup>1</sup> and 
[Sergey Fomel](https://www.jsg.utexas.edu/researcher/sergey_fomel/)<sup>1</sup>.
<sup>1</sup>BEG, UT Austin; <sup>2</sup>Uber.

## Getting Started with Example Model for fault prediction

If you would just like to try out a pretrained example model, then you can download the [pretrained model](...) and use the 'prediction.ipynb' script to run a demo.

### Dataset

**To train our CNN network, we automatically created 200 pairs of synthetic seismic and corresponding fault volumes, which were shown 
to be sufficient to train a good fault segmentation network.** 

**The training and validation datasets can be downloaded [here](...)**

### Training

Run train3 to start training a new faultSeg model by using the 200 synthetic datasets

## Publications

If you find this work helpful in your research, please cite:

    @article{wu2018faultSeg,
        author = {Xinming Wu, Luming Liang, Yunzhi Shi and Sergey Fomel},
        title = {FaultSeg: using synthetic datasets to train an end-to-end CNN for 3D fault segmentation},
        journal = {GEOPHYSICS},
        volume = {submitted},
        number = { },
        pages = { },
        year = {2018},
    }

---
## Test results on multiple field datasets

Although trained by only synthetic datasets, the CNN model works pretty 
well in predicting faults in field datasets that are acquired at 
totally different surveys. 

### Example of Netherlands off-shore F3 (provided by the Dutch Government through TNO and dGB Earth Sciences)

compare the CNN fault probability (top right) with fault likelihood (bottom)
![results/f3CnnFaultByWu.png](results/f3CnnFaultByWu.png)

### Example of Clyde (provided by Clyde through Paradigm)

compare the CNN fault probability (middle) with fault likelihood (right)
![results/clydeCnnFaultByWu.png](results/clydeCnnFaultByWu.png)

### Example of Costa Rica (acquired in the subduction zone, Costa Rica Margin, provided by Nathan Bangs)

compare the CNN fault probability (left column) with fault likelihood (right column)
![results/crfCnnFaultByWu.png](results/crfCnnFaultByWu.png)

### Example of Campos (acquired at the Campos Basin, offshore Brazil, provided by Michacle Hudec)
![results/camposCnnFaultByWu.png](results/camposCnnFaultByWu.png)

### Example of [Kerry-3D](https://wiki.seg.org/wiki/Kerry-3D)
![results/kerryCnnFaultByWu.png](results/kerryCnnFaultByWu.png)
### Example of [Opunake-3D](https://wiki.seg.org/wiki/Opunake-3D)
![results/opunakeCnnFaultByWu.png](results/opunakeCnnFaultByWu.png)

## License

This extension to the Keras library is released under a creative commons license which allows for personal and research use only. 
For a commercial license please contact the authors. You can view a license summary here: http://creativecommons.org/licenses/by-nc/4.0/