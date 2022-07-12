# better-nmt-segmentation

The provided segmentations with the [NMTv2 atlas](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_tempatl/template_nmtv2.html) are pretty problematic and have several inaccuracies, particularly with the white-gray matter boundaries. This contains a hacked together custom .5mm segmentation I ran using various steps inovlving ANTs' N4BiasCorrect, FSL's FAST, and custom routines in Nilearn. 

The NMTv2 is segmented into 4 classes. CSF, gray matter, white matter, and subcortex/cerebellum. The latter was just taken as a binary mask of the SARM parcellation provided with NMTv2. Each class is included as a separate binary mask in `segmentations/`, as well as a complete segmentation image containing all classes.