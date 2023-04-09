This project uses wavelet decomposition, singular value decomposition (SVD), and linear discrimination analysis (LDA) to teach a computer to recognize handwritten digits with high accuracy (99.72% for 0 and 1, and 94% for all 10 digits). SVMs provided the best overall accuracy at 98%.
<h3>Project report CP4.pdf includes all the results and plots</h3>

<!DOCTYPE html>
<html>
  <body>
    <h1>Teaching a Computer to Recognize Written Numbers</h1>
    <p>We’re going to take a subset of Yann LeCun’s famous dataset, which I preprocessed to reduce the amount of busy work. I saved the training datasets as <em>CP4_training_images.mat</em> and <em>CP4_training_labels.mat</em>, and the test datasets as <em>CP4_test_images.mat</em> and <em>CP4_test_labels.mat</em>.</p>
    <p>We will write a few different learning algorithms; some from scratch and some using native MATLAB functions (or associated Python libraries).</p>
    <ol>
      <li>
        <h2>Reshape and take the SVD</h2>
        <ul>
          <li>Reshape the images into column vectors (like the datasets we used in the lecture codes), and take the SVD of the images (like we did in the lecture codes).</li>
          <li>Observe how the singular values decrease. What is a good rank to reconstruct the images? I’ll put more guidance in the code template.</li>
          <li>Play around with the projections: project the data onto three right singular vectors (columns of V).</li>
        </ul>
      </li>
      <li>
        <h2>Linear Discriminant Analysis (LDA)</h2>
        <ul>
          <li>Pick two digits (any two). Use Linear Discriminant Analysis (just like what we did with dogs and cats) to classify them.</li>
          <li>Now do this for three digits.</li>
          <li>Which two digits are hardest to separate using this method? (i.e., which two digits have the highest percentage of data on the wrong side of the threshold)</li>
          <li>Which two digits are the easiest to separate?</li>
        </ul>
      </li>
      <li>
        <h2>Comparsion with other algorithms</h2>
        <ul>
          <li>Now let’s use the built-in MATLAB functions or associated Python libraries for support vector machines (fitcsvm()) and decision tree (fitctree()) to separate the digits.</li>
          <li>How do the three methods compare?</li>
        </ul>
      </li>
    </ol>
  </body>
</html>
