Problem Introduction: 
- Given two images, and no other information, compute matches between the images and the 3D position of the points that generate these matches and the cameras that generate the images
- Given three images, and no other information, compute the matches between images of points and lines, and the position in 3D of these points and lines and the camera
- Compute the epipolar geometry of a stereo rig, and trifocal geometry of a trinocular rig, without requiring a calibration project. 
- Compute the internal calibration of a camera from a sequence of images of natural scenes

These algorithms are uncalibrated. 


Outline: 

Part 0: Background 
- Introduces the central ideas in the projective geometry of 2-space and 3-space. 
- How this geometry may be represented, manipulated and estimated.
- How the geometry relates to various objectives in computer vision such as rectifying images of planes to remove perspective distortion 


Part 1: Single view geometry
- Introduce various cameras that model the perspective projection from 3-space to an image are defined and their anatomy explored. 
- Their estimation using traditional techniques of calibration objects is described
- Camera calibration from vanishing points and vanishing lines


Part 2: Two view geomery
- This part describes the epipolar geometry of two cameras
- Projective reconstruction from image point correspondences
- Methods of resolving the projective ambiguity
- Optimal triangulation 
- Transfer between views via planes

Part 3: Three view geometry
- Introduces the trifocal geometry of three cameras is described
- Transfer of a point correspondence from two views to a third
- Transfer for a line correspondence
- Computation of the geometry from point and line correspondences
- Retrieval of the camera matrices

Part 4: N-views
- Extends three view geometry to four views
- Describes estimation methods application to N-views
- Factorization algorithm of Tomasi and Kanade for computing structure and motion simultaneously from multiple images
- Cover themes that have been "touched on" 🤔 eariler chapters but can be understood more fully and uniformly by emphasising their commonality
- Deriving multi-linear view constraints on correspondences, auto calibration adn ambiguous solutions. 