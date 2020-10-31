
## Dataset:

This dataset consists of around 3500 images containing four main classes:
 - Hard hats
 - Vests
 - Masks
 - Boots

Common settings include construction areas/construction workers, military personnel, traffic policemen etc 
Not all classes are present in an image. Also one image may have many repitions of the same class 
For example, a group of construction workers without helmets, but with vests and boots 

## Explanation:
There are four folders provided:
 - images
 - labels
 - depth
 - planar

### 1. Raw images  
The raw images are present under the images folder. The images were collected by crowdsourcing and do not follow any particular naming convention.   
They are also of varied sizes.    

### 2. Bounding Boxes   
A Yolo compatible annotation tool was used to annotate the classes within these images.   
These are present under the labels folder as text files. However please note that not all raw images have a corresponding label   
A few things to note:  
- Each image can contain 0 or more annotated regions.    
- Each annotated region is defined by four main parameters: x, y, width, height   
- For the rectangular region, (x, y) coordinates refers to top left corner of the bounding box   
- width and height refer to the width and height of the bounding region. The centroid of the bounding box can be calculated from this if required.  
- A label file corresponding to an image is a space separated set of numbers. Each line corresponds to one annotated region in the image.  
- The first column maps to the class of the annotated region (order of the classes is as described above). The other four numbers represent the bounding boxes (ie annotated region), and stand for the x, y, width and height parameters explained earlier. These four numbers should be between 0 and 1. 

    
