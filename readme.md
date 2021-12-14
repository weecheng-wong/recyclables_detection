## Supporting SG Recycling Efforts with Artificial Intelligence

This is part of my Capstone project for General Assembly Data Science Immersive (DSI-SG-25). In this project, I am exploring how AI, specifically computer vision and deep learning could enhance support for Singapore's recycling efforts.

## Background

Singapore's recycling efforts have stagnated in 60% range for the past 10 years. Even as the local waste generation quantity has remained stable through the years, the sole landfill in Semakau is projected to reach its capacity in 2035. There is definitely scope for the 3Rs, namely reduce, reuse and recycle. Here, the focus is on the recycling scope where there are opportunities to leverage AI for support recycling efforts.

## Executive Summary

The main issues plaguing recycling are contamination by food and liquid wastes, and the mixing of recyclables with non-recyclables be it from ignorance or wilful disregard. Because of the way recyclables are commingled in a single recycle bin in Singapore's context, this poses several challenges at the Materials Recovery Facility (MRF) where recyclables are sorted. Recyclables are manually sorted and contaminated materials are discarded into general waste.

An idea could be to leverage Artificial Intelligence to automate the manual sorting process at the MRF. This project does not preclude the ability for such a deployment.

This project seeks for a more lofty ideal - eliminate contamination and improve recyclables quality through sorting at the point of recyclables disposal to minimize down-cycling of recyclable materials.

This could be achieved through 4 main principles - detect, classify, sort, educate.

AI could be trained to detect and classify recyclables. Sorting could be carried out with the support of robotics or perhaps smart funnelling system. The AI can also be a tool to support public education particularly in pre-recycling handling such as cleaning and separating of mixed materials recyclables components (i.e. bottle cap, bottle and label; carton cap and drink carton; etc). The aim is to achieve high recyclables quality and support a circular economy.

## Conclusion

As an initial proof of concept, this project demonstrates the capability of AI to detect and classify different classes of recyclables with reasonable success. It has ~40% accuracy although it is best to visualize results to have a tangible sense of what that means. The detection is no slouch even at such a level, and offers much promise. (refer to pdf slides)

The current model architecture uses Faster R-CNN with ResNet50 FPN as backbone, and provides reasonable good predictive capability despite limited (<40 epochs) training and tuning.

Despite that the training data (images) did not come from local sources, the model is able to generalize somewhat to the Singapore's context for Plastic wastes and recyclables.

There are limitations (refer to pdf slides) which will be addressed in future works.

## Future Works

Further works may be expected post this initial proof of concept for this Capstone project. This repo will be update accordingly.

## Notebooks

You will need to download the dataset (~3GB) via download.py to run the first 3 notebooks (1_data_exploratory / 2_model_training / 3_validation_test).\
You can however, run the 4th notebook (4_preview_results) without the dataset, and feel free to test with your custom images of trash and recyclables.

## References and Resources

[Singapore National Environment Agency (NEA) Recylcing Resources](https://www.nea.gov.sg/our-services/waste-management/3r-programmes-and-resources)\
[CNA article on the challenges of raising Singapore's recycling rate](https://www.channelnewsasia.com/singapore/in-focus-singapore-recycling-sustainability-blue-bins-waste-1339091)\
[TACO Dataset](http://tacodataset.org/)\
[TACO Toolkit](https://github.com/pedropro/TACO)\
[Training Object Detector with custom COCO dataset in Pytorch](https://medium.com/fullstackai/how-to-train-an-object-detector-with-your-own-coco-dataset-in-pytorch-319e7090da5)\
[Pytorch Documentation and Tutorials](https://pytorch.org/docs/stable/index.html)
[How to recognise objects in videos with Pytorch](https://dida.do/blog/how-to-recognise-objects-in-videos-with-pytorch)
