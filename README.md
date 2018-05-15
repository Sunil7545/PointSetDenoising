# PointSetDenoising
NVT-based point set denoising algorithm. 
Sunil Kumar Yadav, Ulrich Reitebuch, Martin Skrodzki, Eric Zimmermann, Konrad Polthier


Constraint-based Point Set Denoising using Normal Voting Tensor and Restricted
Quadratic Error Metrics

Abstract:
In many applications, point set surfaces are acquired by 3D scanners. During this acquisition
process, noise and outliers are inevitable. For a high fidelity surface reconstruction
from a noisy point set, a feature preserving point set denoising operation has
to be performed to remove noise and outliers from the input point set. To suppress these
undesired components while preserving features, we introduce an anisotropic point set
denoising algorithm in the normal voting tensor framework. The proposed method consists
of three different stages that are iteratively applied to the input: in the first stage,
noisy vertex normals, are initially computed using principal component analysis, are
processed using a vertex-based normal voting tensor and binary eigenvalues optimization.
In the second stage, feature points are categorized into corners, edges, and surface
patches using a weighted covariance matrix, which is computed based on the processed
vertex normals. In the last stage, vertex positions are updated according to the processed
vertex normals using restricted quadratic error metrics. For the vertex updates,
we add different constraints to the quadratic error metric based on feature (edges and
corners) and non-feature (planar) vertices. Finally, we show our method to be robust
and comparable to state-of-the-art methods in several experiments.


Requirement:

    Windows 7 or newer.
    
Instructions:

    To compile the provided sourec code:
    
    1. Please extract the folder data.7z.
    
    2. It has five different folders regarding the different models.
    
    3. Each folder has a .bat file (e.g. launcherBallJoint.bat in ballJoint folder).
    
    4. Run this .bat file by double click.
    
    5. It will open a new window with a loaded model.
    
    6. For every model, we fix the parameters in the scroll bars, so you dont have to change them.
    
    7. To compute the noise-free point set, user has to press the smoothing button (point set smoothing).
    
    8. After that this button color will change and algorithm started.
    
    9. current status of the algorithm is displayed in lower left corner of the smoothing window.
   

Output mesh is reconstructed using "ball pivoting algorithm " (in the article). Here, we use the models with intial mesh from geometry to increase visibility of different features. As mesh is from original surface, the output may have some artifacts because we are not optimizing mesh quality during the point set denoising.  
