
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
These are present under the labels folder as text files   


However please note that not all raw images have a corresponding label
