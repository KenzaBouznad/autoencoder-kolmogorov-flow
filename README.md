<div align="center">
  <h1>Autoencoder for Kolmogorov Flow Reconstruction</h1>
  <p><strong>Machine Learning for Dynamical Systems | TU Berlin | Summer Semester 2023</strong></p>
</div>

<hr />

<h2>📌 Project Overview</h2>
<p>
  This project investigates the reconstruction of 2D Kolmogorov Flow velocity fields using 
  <strong>Convolutional Autoencoders</strong> and <strong>Proper Orthogonal Decomposition (POD)</strong>. 
  By analyzing the flow across three different Reynolds numbers, we evaluate how machine learning 
  extracts features from varying levels of turbulence.
</p>



<ul>
  <li><strong>Re=20</strong>: Low turbulence / Laminar state.</li>
  <li><strong>Re=30</strong>: Intermediate turbulence state.</li>
  <li><strong>Re=40</strong>: High complexity fluid dynamics.</li>
</ul>

<h2>🛠️ Tech Stack</h2>
<table style="width:100%">
  <tr>
    <td><strong>Language</strong></td>
    <td>Python</td>
  </tr>
  <tr>
    <td><strong>Libraries</strong></td>
    <td>TensorFlow, Keras, NumPy, Matplotlib</td>
  </tr>
  <tr>
    <td><strong>Methodology</strong></td>
    <td>CNN Autoencoders, POD, Dimensionality Reduction</td>
  </tr>
</table>

<h2>🏗️ Model Architecture</h2>
<p>
  The architecture utilizes a deep convolutional approach to compress high-dimensional fluid snapshots into a low-dimensional latent space:
</p>
<ul>
  <li><strong>Encoder:</strong> Utilizes <code>Conv2D</code> and <code>MaxPooling2D</code> layers for feature extraction.</li>
  <li><strong>Latent Space:</strong> Represents the compressed fluid state (e.g., 8-dimensional for Re=20).</li>
  <li><strong>Decoder:</strong> Employs <code>Conv2DTranspose</code> and <code>UpSampling2D</code> to reconstruct the original velocity fields ($u$ and $v$ components).</li>
</ul>



<h2>📂 Repository Structure</h2>
<ul>
  <li><code>re_20.ipynb</code> - Analysis and model training for Reynolds number 20.</li>
  <li><code>re_30.ipynb</code> - Analysis and model training for Reynolds number 30.</li>
  <li><code>re_40.ipynb</code> - Analysis and high-resolution modeling for Reynolds number 40.</li>
</ul>

<h2>🎓 Authors</h2>
<ul>
  <li><strong>Kenza Bouznad</strong></li>
  <li><strong>Diego Solis</strong></li>
</ul>

<h2>📜 References</h2>
<ol>
  <li>Shebalin, J. V. (1997). <em>Kolmogorov flow in three dimensions.</em></li>
  <li>Weiss, J. (2019). <em>A Tutorial on the Proper Orthogonal Decomposition.</em></li>
</ol>
