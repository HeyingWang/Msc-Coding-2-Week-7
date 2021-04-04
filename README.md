# Msc-Coding-2-Week(7) Use TensorFlow to Creatve Outputs

CCI-CC-S2-In-class exercise by Heying Wang

## Intro 

  This exercise focus on using TensorFlow to create outputs

## Technology used for implementation

 ### Neural style transfer
This is implemented by optimizing the output image to match the content statistics of the content image and the style statistics of the style reference image. These statistics are extracted from the images using a convolutional network.
 

## Design Process
   Import and configure modules->Visualize the input-> **trying Fast Style Transfer using TF-Hub** -> 
   **original style-transfer algorithm**
   1. I have changed the `steps_per_epoch`  to change the `Train steps`  for getting the output as:
   `Train step: 500
    Total time: 285.2` 
   2. I also decrease the high frequency artifacts by **total variation loss**
   3. At last I rerun the optimization using the  `total_variation_weight = 25` and  include it in the train_step function and get the result 
     `Train step: 500
      Total time: 275.8` 

## Further improvement
   Modify and optimise models to produce images with the desired quality and atmosphere
  

## References
 • content image: https://jasminewhy.files.wordpress.com/2021/04/leon-contreras-va5ohgk8hke-unsplash.jpg
 • style image: https://upload.wikimedia.org/wikipedia/commons/1/15/Vincent_van_Gogh_-_Wheat_Field_with_Cypresses_%28National_Gallery_version%29.jpg

## Related link
 • Learning Resource https://www.tensorflow.org/tutorials/generative/style_transfer


