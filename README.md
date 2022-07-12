# better-nmt-segmentation

The provided segmentations with the [NMTv2 atlas](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_tempatl/template_nmtv2.html) is pretty problematic and has several inaccuracies, particularly with the white-gray matter boundary. This contains a hacked together custom .5mm segmentation I ran using various steps inovlving ANTs' N4BiasCorrect, FSL's FAST, and custom routines in Nilearn. 
