---
layout: page
title: Boundary Equilibrium GANs
description: 
img: /assets/img/BEGAN.png
---
GAN training is rife with problems such as non-convergence(model parameters never converge), model collapse(limited sample variety), diminished gradient(discriminator pushes down on the generator that it learns nothing)  

[BEGAN](https://www.semanticscholar.org/paper/BEGAN%3A-Boundary-Equilibrium-Generative-Adversarial-Berthelot-Schumm/6b95a3dbec92071c8552576930e69455c70e529c) is an autoencoder based GAN trained using Wasserstein distance and has ideas borrowed from control theory infused into the process. It essentially balances the generator and discriminator during training and provides an approximate measure of convergence and tunable image diversity and quality, 

<div class="img_row">
    <img class="col two left" src="{{ site.baseurl }}/assets/img/BEGAN.png" alt="" title="Reference Pic only"/>
</div>

---
 [https://github.com/AshVijay/BEGAN.git](https://github.com/AshVijay/BEGAN.git)
---
