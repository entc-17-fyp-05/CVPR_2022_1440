# Part semantic aware latent space navigation for controlled regeneration of 3Dpoint clouds

* * *

**This is the official code repository of the CVPR submission - Paper ID 1440**

* * *
GIF
<!-- Enter gif and explain -->

* * *

### Installation

##### **Step 01** : Install the conda enviroment

<!-- insert steps -->
* * *

### Datasets and Pre-Trained Models

#### **Step 01** : Download the datasets
    Datasets are available at *|url|*
    Download and place them at the path "Final_Repository/data"

#### **Step 02** : Download the Trained Models
    Pre-Trained models are available at *|url|*

    Download and place them at the path "Final_repository/models/*--model--*/Trained_models"

    You can find pre-trained models of the following
        1. PointNet Part Segmentation
        2. 3DAAE
        3. Pointflow
        4. Diffusion Probabilitic Models
        
* **Example** : If you want to edit pointclouds with the **Diffusion Probabilistic Model** for the **chair class** you will need the following:*

        data : chair_parts.npy | chair_objects.npy

        pre-trained models : AAE_chair_parts.pth | chair.pth | latent_con_model.pth | DPM_chair_objects.pt 

* * *

### Editing Framework

Run the notebook "Final_Experiments2.ipynb" from the begining. The customized entries need to specified at the mentioned places in the notebook. You will have to specify the object category, Root DIR, Generative Model and the optimum number of clusters based on the Davies Bouldin score. The respective locations and instructions are specified in the notebook.

* * *

### Credits

#### 3DAAE

[code](https://github.com/MaciejZamorski/3d-AAE) [paper](https://arxiv.org/abs/1811.07605)

    @article{Zamorski20203dAAE,
      year = {2020},
      month = {April},
      volume = {193},
      articles= {102921},
      author = {Maciej Zamorski and Maciej Zi{\k{e}}ba and Piotr Klukowski and Rafa{\l} Nowak and Karol Kurach and Wojciech Stokowiec and Tomasz Trzci{\'{n}}ski},
      title = {Adversarial autoencoders for compact representations of 3{D} point clouds},
      journal = {Computer Vision and Image Understanding}
    }

#### Pointflow

[code](https://github.com/stevenygd/PointFlow) [paper](https://arxiv.org/abs/1906.12320)

    @InProceedings{guandao2020pointflow,
    author = {Yang, Guandao and Huang, Xun and Hao, Zekun and Liu, Ming-Yu and Belongie, Serge and Hariharan, Bharath},
    title = {PointFlow: 3{D} Point Cloud Generation With Continuous Normalizing Flows},
    booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
    month = {October},
    year = {2019}
    }

#### Diffusion Probabilistic Models

[code](https://github.com/luost26/diffusion-point-cloud) [paper](https://arxiv.org/abs/2103.01458)

    @inproceedings{luo2021diffusion,
      author = {Luo, Shitong and Hu, Wei},
      title = {Diffusion Probabilistic Models for 3D Point Cloud Generation},
      booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
      month = {June},
      year = {2021}
    }







