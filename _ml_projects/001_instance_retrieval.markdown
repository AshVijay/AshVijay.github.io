---
layout: page
title: Instance Retrieval from Video Sources
description: A sparse coding approach for efficient object instance retrieval from videos
img: /assets/img/obj_ret_1.jpg
---


This is an implementation of Tan Yu, et Al's paper [https://www.ijcai.org/proceedings/2017/0635.pdf](https://www.ijcai.org/proceedings/2017/0635.pdf) using Pytorch. The bounding box proposals used for training are generated using an openCV implementation of [EdgeBoxes](https://pdollar.github.io/files/papers/ZitnickDollarECCV14edgeBoxes.pdf).
Mongodb serves as a scalable data store to retain the object proposals indexed by video frames. For each video, we learn a reconstruction model(based on K-Sparse autoencoders) that reconstructs all the proposals.
In the test phase, the query image is reconstructed iteratively and the model that reconstructs it the best, would likely contain the object. 

<div class="img_row">
     <img class="col two centre" src="{{ site.baseurl }}/assets/img/obj_ret_3.png" alt="" title="Results"/>
</div>




---
**Github Link:** [https://github.com/AshVijay/Instance-retrieval-from-video-sources](https://github.com/AshVijay/Instance-retrieval-from-video-sources)
---
