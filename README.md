🖌️ Realistic CSS Paint Roller Loader
This repository hosts a high-fidelity, purely CSS-driven loading animation designed to mimic the realistic application of paint using a roller. Optimized for web deployment, this loader provides engaging visual feedback during asynchronous operations, suitable for high-end web applications and portfolios.
Key Features
This animation moves beyond standard, repetitive loaders by incorporating complex visual and behavioral details:
Realistic Motion & Timing: The stroke motion runs on a deliberate 4-second loop with continuous vertical movement, providing a fluid sense of ongoing work rather than a frantic pulse.
Painter's Arc Simulation: Each of the three vertical strokes uses transform: skewX() and translateX() within the keyframes to simulate the slight horizontal arc caused by a painter's fixed arm pivot point.
Random Density & Grain: The paint application avoids uniformity by using unique opacity values across three distinct strokes (0.65, 0.75, 0.85) to simulate random density and uneven roller loading. A background linear-gradient provides an authentic grainy, first-coat texture.
Randomized Drips: Three separate drip elements (paint-drip) are timed with randomized animation-delay and animation-duration properties, ensuring drips fall randomly across the main 4-second cycle for a natural, non-synchronized effect.
Seamless Loop: Keyframe resets are instantaneous and invisible, ensuring a smooth, non-janky, continuous loop ideal for a long-duration loading indicator.
🛠️ Installation and Setup
This is a lightweight, dependency-free implementation. No complex build tools or frameworks are required.
Clone the Repository: Get the files onto your device using your preferred Git client.
File Structure: Ensure the following three files are located in the same directory:
index.html (The structure containing the elements)
style.css (The complete animation logic)
paint-roller-icon.png (The custom image asset)
Integration: To use this loader in your main project:
Copy the content of the HTML structure (.animation-container and its children) into the section of your main page where the loader should display.
Link the CSS file in your HTML <head>:
<link rel="stylesheet" href="path/to/style.css">
Customization
The design is highly flexible for rapid adaptation:
Property
File
Recommended Adjustment
Animation Speed
style.css
Modify animation: ... 4s ... to a faster (e.g., 2.5s) or slower time.
Paint Color
style.css
Change the background-color in the .paint-stroke class (currently #80dee6).
Density (Opacity)
style.css
Adjust the opacity values in .stroke-1, .stroke-2, etc., between 0.0 and 1.0.
Loader Size
style.css
Adjust width and height of .animation-container. Note: Keyframe heights must be adjusted accordingly.
📄 License
This project is open source and available under the MIT License.
