# 2D/3D object tracing and interpretable seperation  
## information and background
aim：high accuracy+high speed  
definition of object tracing：give the initial position of aim object，locate and trace it   
challenge：noise in the background; image deforms greatly  

## basic model  
model: ASKCF(adaptive Scala Kernel Correlation Filter)  
result: tracing reslut good for 2.3mm object; descriptor will largely influenced the result  

## improvement   
### 2D dimension  
improvement model: DCFNET(discriminative Correlation Filter Network); pick out simple features from frond layer  
improvement model: multiDCFNET; apply to more than one object while improve the tracing accuracy and robustness  

### 3D dimension  
improvement：SSPMNET(Siamese Spatial Pyramid Matching Network)；find separation according to semantic feature understanding  
improvement：Tri-planar DCFNET；grid searching can prove the insistence between the movement of objects and force  

## future work
Extension：attention segmet（segmention network with attention mechanism）；correlations between different features can be expressed as medical regulation
