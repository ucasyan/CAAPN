# CAAPN

Crowd localization aims to predict the positions of humans in images of crowded scenes. While existing methods have made significant progress, two primary challenges remain: (i) a fixed number of evenly distributed anchors can cause excessive or insufficient predictions across regions in an image with varying crowd densities, and (ii) ranking inconsistency of predictions between the testing and training phases leads to the model being sub-optimal in inference.
To address these issues, we propose a Consistency-Aware Anchor Pyramid Network (CAAPN) comprising two key components: an Adaptive Anchor Generator (AAG) and a Localizer with Augmented Matching (LAM). 
The AAG module adaptively generates anchors based on estimated crowd density in local regions to alleviate the anchor deficiency or excess problem. 
It also considers the spatial distribution prior to heads for better performance.
The LAM module is designed to augment the predictions which are used to
optimize the neural network during training by introducing an extra set of target candidates and correctly matching them to the ground truth.
The proposed method achieves favorable performance against state-of-the-art approaches on five challenging datasets: ShanghaiTech A and B, UCF-QNRF, JHU-CROWD++, and NWPU-Crowd.
