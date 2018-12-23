# PicsArt-Hack-binary_segmentation

The goal of the hackathon was to build a solution for image processing which can be helpful for [PicsArt](https://picsart.com/?hl=en) applications.  
Here I publish results for the first stage: segmenting people on photos.
PicsArt gives us labeled [dataset](https://drive.google.com/file/d/1_e2DcZnjufx35uSmQElN5mpdo-Rlv7ZI/view?usp=sharing).  
[Dice](https://en.wikipedia.org/wiki/S%C3%B8rensen%E2%80%93Dice_coefficient) coef. was used as evaluation metric.  

[MobileNetV2 model](https://drive.google.com/file/d/1mMtNNPRvc7DVC-Ozu2ne5cXaOrVNY7Dm/view?usp=sharing)  

resnet101: 44,549,160
mobilenetV2: 6,906,767

photos 320x256

437 ms cpu mobilenetv2
2140 ms cpu resnet101
~5x slower

24 ms gpu mobilenetv2
43 ms gpu resnet101
~2x slower
