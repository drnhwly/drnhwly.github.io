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
</style>

<div class="gallery">
  <img src="assets/images/image1.jpg" alt="Description of image 1">
  <img src="assets/images/image2.jpg" alt="Description of image 2">
  <img src="assets/images/image3.jpg" alt="Description of image 3">
  </div>
