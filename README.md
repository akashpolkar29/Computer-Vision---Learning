# Computer-Vision-Learning
Daily progress and learning
<br>
## Challenegs in Computer Vision to detect the objects from the picture
<br>
  a. Viewpoints
<br>
  b. Camera Limitations
<br>
  c. Lighting
<br>
  d. Scaling
  <br>
  e. Object Variation
<br>

## Understanding Digital Image Representation  
1. **How Humans Perceive Color**:  
   - Light reflected from objects falls within the visible spectrum (400–700 nm).  
   - Example: Yellow light has a wavelength of 570–580 nm, interpreted by the optic nerve and visual cortex.  

2. **Digital Representation of Images**:  
   - Images are composed of **pixels**, where each pixel holds a value:  
     - **Grayscale Images**: Values range from 0 (black) to 255 (white), with intermediate values representing shades of gray.  
     - **Color Images (RGB)**:  
       - Each pixel has three values (Red, Green, Blue).  
       - Each channel (R, G, B) ranges from 0 to 255.  
       - Example:  
         - Pure Red: `(255, 0, 0)`  
         - Pure Green: `(0, 255, 0)`  
         - Yellow (Red + Green): `(255, 255, 0)`.  

3. **Binary Representation of Pixel Values**:  
   - Pixel values are stored in binary (e.g., `255 = 11111111`).  
   - Grayscale images use 8-bit depth, while color images use 24-bit depth (8 bits per channel for R, G, and B).  

4. **Image Storage**:  
   - Grayscale images have a single matrix of pixel values.  
   - Color images have three matrices (one for each channel: R, G, and B), combined to form the final image.  

5. **Color Mixing**:  
   - Combining values of R, G, and B channels creates a variety of colors visible to humans.  

### Applications  
- Understanding pixel representation is essential for building machine learning algorithms for tasks like:  
  - Image manipulation.  
  - Lane detection in self-driving cars.  
  - Traffic sign classification using RGB values.  
