# My Photos
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

.masonry-grid {
  /* Sets the number of columns and the gap between them */
  column-count: 3;
  column-gap: 20px; 
}

.masonry-grid img {
  /* Breaks the images out of their regular flow and places them into columns */
  break-inside: avoid;
  /* Makes the image span the entire width of its column */
  width: 100%; 

  border-radius: 8px; /* Adjust this value for more or less rounded corners */
  margin-bottom: 20px; /* Add some vertical space between images */
  
  /* Removes any bottom margin or spacing that might cause gaps */
  display: block; 
}
</style>

<div class="masonry-grid">
  <a href="assets/images/image1.jpg" data-lightbox="gallery">
    <img src="assets/images/image1.jpg" alt="Image description">
  </a>
  <a href="assets/images/image2.jpg" data-lightbox="gallery">
    <img src="assets/images/image2.jpg" alt="Image description">
  </a>
  <a href="assets/images/image3.jpg" data-lightbox="gallery">
    <img src="assets/images/image3.jpg" alt="Image description">
  </a>
  <a href="assets/images/image4.jpg" data-lightbox="gallery">
    <img src="assets/images/image4.jpg" alt="Image description">
  </a>
  <a href="assets/images/image5.jpg" data-lightbox="gallery">
    <img src="assets/images/image5.jpg" alt="Image description">
  </a>
  <a href="assets/images/image6.jpg" data-lightbox="gallery">
    <img src="assets/images/image6.jpg" alt="Image description">
  </a>
  <a href="assets/images/image7.jpg" data-lightbox="gallery">
    <img src="assets/images/image7.jpg" alt="Image description">
  </a>
  <a href="assets/images/image8.jpg" data-lightbox="gallery">
    <img src="assets/images/image8.jpg" alt="Image description">
  </a>
</div>
