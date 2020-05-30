## Highly Accurate Scale Estimation from Multiple Keyframes using RANSAC Plane Fitting with a Novel Scoring Method
Additional experimental results for the paper titled above.
### Abstract
Due to the purely projective nature of a single camera, monocular visual simultaneous localization and mapping~(vSLAM) algorithms suffer from scale drift. Recent studies have addressed the scale drift problem by estimating the height of the camera from the ground plane. Specifically, the well-known random sample consensus~(RANSAC) algorithm is applied to the reconstructed three-dimensional ground points (3DGPs) to find the ground plane. In RANSAC, a fitted plane is evaluated by counting the number of inlier 3DGPs whose point-to-plane distance is less than a predefined threshold. However, owing to the low accuracy of 3DGP reconstruction, the fitted plane may be inaccurate for scale estimation. In addition, the number of 3DGPs reconstructed from the textureless ground region is often insufficient for robust estimation. To overcome these problems, in this paper, we collect a large number of 3DGPs across multiple frames based on the assumption that if the captured images share a sufficient number of feature points, the vehicle is driving on a flat surface. Moreover, we introduce a novel accuracy measure of the fitted plane. Specifically, from the previous keyframe, we first obtain the 3D points from the intersection of the fitted plane with a ray passing through the camera center and the two-dimensional (2D) feature points detected on the ground region. We then transform the 3D points on the plane and 2D feature points to the coordinate system of the current keyframe using their respective planar homography transformation. Finally, we project the transformed 3D points onto the image plane of the current keyframe and measure the average Euclidean distance between the projected points and the transformed feature points. This average Euclidean distance is measured during RANSAC iterations, and the camera height is obtained from the fitted plane that has the smallest distance. ORB-SLAM with the proposed scale estimation method achieves the average translation error of 1.05\% on the KITTI dataset, which outperforms the state-of-the-art monocular vSLAM methods.

### Recorded video for sequence 00
### Recorded video for sequence 02
### Recorded video for sequence 03
### Recorded video for sequence 04
### Recorded video for sequence 05
### Recorded video for sequence 06
### Recorded video for sequence 07
{% include sequence07.html%}
### Recorded video for sequence 08
### Recorded video for sequence 09
### Recorded video for sequence 10
### Support or Contact
