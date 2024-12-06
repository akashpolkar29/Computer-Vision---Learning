# Image Transformations and Perspective Transformation with OpenCV

## 1. Image Transformations Overview:
- Learned essential image manipulation techniques: **rotation**, **translation**, **scaling (resizing)**, **affine**, and **non-affine (perspective) transformations**.
- These transformations are fundamental for tasks like **lane detection**, **object tracking**, and **image pre-processing** in computer vision.

## 2. Affine vs Non-Affine Transformations:
- **Affine Transformation**: Preserves **parallel lines** and maintains the geometry of the image.
- **Non-Affine (Projective) Transformation**: Alters parallel lines, changing their angles, which is useful for perspective correction.

## 3. Rotation:
- Used `cv2.getRotationMatrix2D()` to create a rotation matrix, specifying the **center**, **angle**, and **scale** (resize factor).
- Applied the rotation using `cv2.warpAffine()` to rotate the image by a specified angle around a defined center.

## 4. Translation:
- Created a **translation matrix** to shift images in the **X** and **Y** directions.
- Applied the translation using `cv2.warpAffine()` to move the image by the specified pixel values.

## 5. Resizing:
- Used `cv2.resize()` to scale images up or down based on the **fx** and **fy** parameters (scaling factors for width and height).
- Applied **cubic interpolation** for smooth scaling without significant quality loss.

## 6. Perspective Transformation:
- **Perspective transformation** changes the viewpoint of an image to make objects appear as if viewed from a different angle, typically from the front.
- Essential for self-driving car applications where images need to be rectified for accurate object detection.

## 7. Source and Destination Points for Perspective Transformation:
- **Source points**: Key points in the original image that define the object (e.g., corners of a sign).
- **Destination points**: Where the transformed image should appear (e.g., front view of the object).
- Calculated the **transformation matrix** using `cv2.getPerspectiveTransform()` and applied it using `cv2.warpPerspective()` to achieve the transformed image.

## 8. Applications of Perspective Transformation:
- **Self-driving cars**: Correcting the perspective of road signs or objects in images for better detection and classification.
- **Template Matching**: Combined with perspective transformation, it enables automatic object detection and transformation in real-time.

## 9. Key Concepts:
- **Affine Transformations**: Maintain parallel lines.
- **Perspective Transformations**: Can distort parallel lines and angles to make objects appear from a different viewpoint.
- Perspective transformation is **critical** for preprocessing images, particularly in **autonomous vehicles** where accurate interpretation of objects from various angles is required.
