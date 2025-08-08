# My Photos
![Bird and Wires](assets/images/20220318_bird_wires.jpg)

<style>
  /* Basic CSS for the photo grid */
  .gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 15px;
  }
  .gallery img {
    width: 100%;
    height: auto;
    border-radius: 8px; /* Optional: adds rounded corners */
    box-shadow: 0 4px 8px rgba(0,0,0,0.1); /* Optional: adds a subtle shadow */
    transition: transform 0.2s; /* Optional: adds a hover effect */
  }
  .gallery img:hover {
    transform: scale(1.05);
  }

.image-gallery {
  display: flex; /* Enables Flexbox */
  flex-wrap: wrap; /* Allows images to wrap to the next line */
  gap: 0; /* Removes all gaps between images */
}

.image-gallery img {
  /* This is the key property for the justified layout.
     It tells the images to grow or shrink to fill the row. */
  flex-grow: 1; 

  /* Ensures images maintain their aspect ratio */
  object-fit: cover; 

  /* Sets a minimum width for each image, preventing them from becoming too small */
  min-width: 200px; 
}

/* This is a crucial trick to ensure the last row is also justified. 
   It adds a flexible empty space to fill the remaining room. */
.image-gallery::after {
  content: '';
  flex-grow: 999999999; /* A very high number to force it to take all remaining space */
}
</style>

<div class="image-gallery">
  <img src="assets/images/image1.jpg" alt="Description of image 1">
  <img src="assets/images/image2.jpg" alt="Description of image 2">
  <img src="assets/images/image3.jpg" alt="Description of image 3">
  <img src="assets/images/image4.jpg" alt="Description of image 4">
  <img src="assets/images/image5.jpg" alt="Description of image 5">
  <img src="assets/images/image6.jpg" alt="Description of image 6">
  <img src="assets/images/image7.jpg" alt="Description of image 7">
  <img src="assets/images/image8.jpg" alt="Description of image 8">
  </div>
