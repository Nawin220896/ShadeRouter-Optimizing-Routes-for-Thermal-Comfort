# ShadeRouter: Optimizing Routes for Thermal Comfort 🚴‍♀️🌳🌞

---

## Authors
- **Mithun Shivakoti**
- **Phaneendra Gavara**
- **Yoshita Yajjapurapu**
- **Naveen Kumar Manokaran**

---

## ✨ Abstract
ShadeRouter is a novel route planning system designed to address the growing concerns of heat exposure in metropolitan areas, especially for cyclists and pedestrians. The system integrates shaded areas into a multi-layered road graph using advanced segmentation models applied to high-resolution satellite images. By leveraging a modified Dijkstra algorithm, ShadeRouter enables users to customize their routes based on a balance of distance and shade coverage. Preliminary tests in Tempe, Arizona, demonstrate its efficacy in enhancing outdoor comfort and promoting sustainable urban mobility.

---

## ✨ Key Features

### 🌟 Core Innovations
1. **Dynamic Shaded Route Planning**:
   - Combines user preferences with dynamic shade data for personalized route optimization.
2. **Satellite Image Segmentation**:
   - Uses models like the Segment Anything Model (SAM) and ControlNet for accurate shade detection.
3. **Multi-Layered Graph Integration**:
   - Incorporates shade data into traditional road graphs to enable shade-prioritized routing.
4. **Modified Dijkstra Algorithm**:
   - Allows flexible trade-offs between distance and shade coverage.

### 🛰️ Dataset
- **Total Images**: 2,925 3D simulated images of Tempe, Arizona.
- **Types**:
  - Satellite images.
  - 3D simulated images with and without sunlight at various times (6 AM to 6 PM).
- **Purpose**:
  - Train and test segmentation models to dynamically extract shade information.

### 🚀 Applications
- Reduces heat exposure for cyclists and pedestrians.
- Enhances urban mobility with sustainability and comfort in mind.
- Adaptable to different urban environments globally using publicly available satellite imagery.

---

## ✨ Methodology

1. **Data Preparation**:
   - Use ControlNet and Stable Diffusion for precise shade segmentation.
   - Incorporate satellite images, building outlines, and edge maps for improved segmentation accuracy.

2. **Dynamic Shade Modeling**:
   - Simulate shade variations across different times of the day.
   - Integrate segmentation outputs into a road graph.

3. **Route Optimization**:
   - Implement a modified Dijkstra algorithm for shade-distance trade-offs.
   - Provide real-time, user-centric routing recommendations.

4. **Evaluation**:
   - Metrics: Structural Similarity Index (SSIM) and Mean Squared Error (MSE).
   - Results: Average SSIM of 0.383 and MSE of 45.76, with model performance improving over time.

---

## ✨ Results

- **Performance**:
  - Effective shade extraction and routing using segmentation models.
  - Demonstrated improvements in user comfort and safety during peak heat hours.
- **Visual Outputs**:
  - Dynamic shade maps and optimized routes for Tempe, Arizona.
  - Comparative analyses of model performance metrics over time.

---

## ✨ Future Work
**Enhanced Shade Simulation**:
Incorporate dynamic weather data and temporal fluctuations.
**Scalability**:
Test on diverse urban layouts and climates.
**Model Improvements**:
Experiment with alternative architectures and diffusion models.
**Public Accessibility**:
Develop a user-friendly app for real-time shade-optimized routing.
