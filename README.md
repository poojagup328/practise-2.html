<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Pooja Plastic Store</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.5/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-SgOJa3DmI69IUzQ2PVdRZhwQ+dy64/BUtbMJw1MZ8t5HZApcHrRKUc4W0kG879m7" crossorigin="anonymous">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
 <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.5/dist/js/bootstrap.bundle.min.js" integrity="sha384-k6d4wzSIapyDyv1kpU366/PK5hCdSbCRGRCMv+eplOQJWyd1fbcAu9OCUj5zNLiq" crossorigin="anonymous"></script>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background: #f4f4f9;
      color: #333;
    }
    header {
      background: linear-gradient(to right, #00bcd4, #009688);
      color: white;
      padding: 1rem;
      text-align: center;
    }
    header h1 {
      margin: 0;
    }
    .contact {
      font-size: 0.9rem;
    }
    .slider {
      width: 100%;
      overflow: hidden;
      position: relative;
    }
    .slider img {
      width: 100%;
      display: block;
    }
    .filter {
      text-align: center;
      margin: 1rem;
    }
    
    .like-btn {
      background-color: #e91e63;
      color: white;
      border: none;
      padding: 0.5rem 1rem;
      border-radius: 8px;
      cursor: pointer;
      margin-top: 0.5rem;
      font-size: 1rem;
    }
    .like-btn:disabled {
      background-color: #9e9e9e;
      cursor: not-allowed;
    }
    .ratings {
      background: #fff8e1;
      padding: 1.5rem;
      text-align: center;
      margin: 2rem auto;
      max-width: 600px;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }
    .stars span {
      font-size: 2rem;
      color: #ccc;
      cursor: pointer;
      transition: color 0.3s ease;
    }
    .stars span.selected {
      color: #ffca28;
    }
    footer {
      text-align: center;
      padding: 1rem;
      background: #009688;
      color: white;
    }
    .d-block{
    
    width: 100%;
    max-height: 600px;
    object-fit: cover;
   border-radius: 12px;
        }
        .social-icons {
            margin: 20px;
        }
        .social-icons a {
            text-decoration: none;
            color: #333;
            margin: 0 15px;
            font-size: 30px;
            transition: color 0.3s;
        }
        .social-icons a:hover {
            color: #4CAF50;
        }
        .item-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            padding: 20px;
            max-width: 1000px;
            margin: auto;
        }
        .item-box {
            background: white;
            border: 1px solid #ccc;
            border-radius: 10px;
            padding: 10px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .item-box img {
            width: 100%;
            height: 120px;
            object-fit: cover;
            border-radius: 5px;
        }
        .item-box h3 {
            font-size: 16px;
            margin: 10px 0 5px;
        }
        .item-box p {
            font-size: 14px;
            color: #555;
        }

  </style>
  <script>
    function toggleLike(btn) {
        btn.classList.toggle('liked');
    }
</script>
</head>
<body>
  <header>
    <h1>Pooja Plastic Store</h1>
    <p class="contact">Owner: Chandan Gupta | 📞 9825202874 | 📍 MahaGadhimai Bariyarpur Bazar Bara, Nepal</p>
  </header>

 


<div id="carouselExampleIndicators" class="carousel slide">
    <div class="carousel-indicators">
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="https://c8.alamy.com/comp/FG3AW0/roadside-stall-selling-plastic-ware-new-market-dhaka-bangladesh-FG3AW0.jpg" class="d-block " alt="...">
      </div>
      <div class="carousel-item">
        <img src="https://c8.alamy.com/comp/T0F2T8/products-from-plastic-ware-objects-take-care-of-plants-on-a-supermarket-showcase-replacing-disposable-tableware-T0F2T8.jpg" class="d-block" alt="...">
      </div>
      <div class="carousel-item">
        <img src="https://c8.alamy.com/comp/FG3AW0/roadside-stall-selling-plastic-ware-new-market-dhaka-bangladesh-FG3AW0.jpg" class="d-block" alt="...">
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>





  <div class="filter">
    <label for="categoryFilter">Filter by Category: </label>
    <select id="categoryFilter" onchange="filterProducts()">
      <option value="all">All</option>
      <option value="buckets">Buckets</option>
      <option value="containers">Containers</option>
      <option value="chairs">Chairs</option>
      <option value="supli">supli</option>
      <option value="harpic">harpic</option>
    </select>
  </div>
  <div class="item-container">
    <div class="item-box">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT2xV93oSqT-kDXdmNS_MMmMUgL5KpSWHMSPQ&s://via.placeholder.com/150" alt="Plastic Chair">
        <h3>Plastic Chair</h3>
        <p>Rs. 500</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://img.drz.lazcdn.com/static/np/p/c2e62990b6b476635231e9a835d9a4c2.jpg_720x720q80.jpg" alt="Plastic Chair">
        <h3>Storage Box</h3>
        <p>Rs. 350</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://5.imimg.com/data5/VZ/WS/AD/SELLER-2908576/20-ltr-plastic-bucket-500x500.JPG" alt="Plastic Chair">
        <h3>Plastic Bucket</h3>
        <p>Rs. 150</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://np-live-21.slatic.net/kf/S12b21053483a4530adc4fcd3806e733dx.jpg" alt="Plastic Chair">
        <h3>Plastic Table</h3>
        <p>Rs. 700</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://m.media-amazon.com/images/I/61DWVSOxqqL.jpg" alt="Plastic Chair">
        <h3>Water Jug</h3>
        <p>Rs. 200</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://crayonscorp.com.np/cdn/shop/files/ddustbin.png?v=1716197383" alt="Plastic Chair">
        <h3>Dustbin</h3>
        <p>Rs. 300</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://images-cdn.ubuy.co.in/6462ff510fda146cfe4057b3-efish-10pcs-rectangle-plastic-portion.jpg" alt="Plastic Chair">
        <h3>Food Container</h3>
        <p>Rs. 180</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://www.tidyhomz.com/wp-content/uploads/2021/05/mug-1-ltr-set-of-6-1.jpg" alt="Plastic Chair">
        <h3>Plastic Mug</h3>
        <p>Rs. 60</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://s.alicdn.com/@sc04/kf/H3ae5d2c047f241af95d08e32a3674844p.jpg_300x300.jpg" alt="Plastic Chair">
        <h3>Water Drum</h3>
        <p>Rs. 800</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://5.imimg.com/data5/SELLER/Default/2022/4/EI/EK/WK/72079282/plastic-kitchen-racks-500x500.JPG" alt="Plastic Chair">
        <h3>Storage Rack</h3>
        <p>Rs. 950</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>



    <div class="item-box">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT2xV93oSqT-kDXdmNS_MMmMUgL5KpSWHMSPQ&s://via.placeholder.com/150" alt="Plastic Chair">
        <h3>Plastic Chair</h3>
        <p>Rs. 500</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://img.drz.lazcdn.com/static/np/p/c2e62990b6b476635231e9a835d9a4c2.jpg_720x720q80.jpg" alt="Plastic Chair">
        <h3>Storage Box</h3>
        <p>Rs. 350</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://5.imimg.com/data5/VZ/WS/AD/SELLER-2908576/20-ltr-plastic-bucket-500x500.JPG" alt="Plastic Chair">
        <h3>Plastic Bucket</h3>
        <p>Rs. 150</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://np-live-21.slatic.net/kf/S12b21053483a4530adc4fcd3806e733dx.jpg" alt="Plastic Chair">
        <h3>Plastic Table</h3>
        <p>Rs. 700</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://m.media-amazon.com/images/I/61DWVSOxqqL.jpg" alt="Plastic Chair">
        <h3>Water Jug</h3>
        <p>Rs. 200</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://crayonscorp.com.np/cdn/shop/files/ddustbin.png?v=1716197383" alt="Plastic Chair">
        <h3>Dustbin</h3>
        <p>Rs. 300</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://images-cdn.ubuy.co.in/6462ff510fda146cfe4057b3-efish-10pcs-rectangle-plastic-portion.jpg" alt="Plastic Chair">
        <h3>Food Container</h3>
        <p>Rs. 180</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://www.tidyhomz.com/wp-content/uploads/2021/05/mug-1-ltr-set-of-6-1.jpg" alt="Plastic Chair">
        <h3>Plastic Mug</h3>
        <p>Rs. 60</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://s.alicdn.com/@sc04/kf/H3ae5d2c047f241af95d08e32a3674844p.jpg_300x300.jpg" alt="Plastic Chair">
        <h3>Water Drum</h3>
        <p>Rs. 800</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
    <div class="item-box">
      <img src="https://5.imimg.com/data5/SELLER/Default/2022/4/EI/EK/WK/72079282/plastic-kitchen-racks-500x500.JPG" alt="Plastic Chair">
        <h3>Storage Rack</h3>
        <p>Rs. 950</p>
        <button class="like-btn" onclick="toggleLike(this)"><i class="fas fa-heart"></i></button>
  
    </div>
</div>


  <section class="ratings">
    <h2>Rate Our Website</h2>
    <div class="stars">
      <span data-value="1">★</span>
      <span data-value="2">★</span>
      <span data-value="3">★</span>
      <span data-value="4">★</span>
      <span data-value="5">★</span>
    </div>
    <p id="rating-output"></p>
  </section>

  <footer>
    <div class="social-icons">
      <a href="https://www.instagram.com/" target="_blank"><i class="fab fa-instagram"></i></a>
      <a href="9825202874" target="_blank"><i class="fab fa-whatsapp"></i></a>
      <a href="https://www.facebook.com/share/193FmRxHPd/" target="_blank"><i class="fab fa-facebook"></i></a>
      <a href="https://www.tiktok.com/" target="_blank"><i class="fab fa-tiktok"></i></a>
  </div>
    &copy; 2025 Pooja Plastic Store. All rights reserved.
  </footer>

  <script>
    // Filter products by category
    function filterProducts() {
      const selectedCategory = document.getElementById("categoryFilter").value;
      const items = document.querySelectorAll(".item-box");
  
      items.forEach((item) => {
        const category = item.dataset.category;
        item.style.display =
          selectedCategory === "all" || selectedCategory === category
            ? "block"
            : "none";
      });
    }
  
    // Toggle Like button state
    function toggleLike(btn) {
      const liked = btn.classList.toggle("liked");
      btn.innerHTML = liked ? '<i class="fas fa-heart"></i> Liked' : '<i class="fas fa-heart"></i>';
      btn.style.backgroundColor = liked ? "#762525" : "#e91e63";
    }
  
    // Handle rating system
    function setupRatings() {
      const stars = document.querySelectorAll(".stars span");
      const output = document.getElementById("rating-output");
  
      stars.forEach((star) => {
        star.addEventListener("click", () => {
          const rating = parseInt(star.dataset.value);
          stars.forEach((s, index) => {
            s.classList.toggle("selected", index < rating);
          });
          output.textContent = `Thanks for rating us ${rating} star${rating > 1 ? "s" : ""}! ${"⭐".repeat(rating)}`;
        });
      });
    }
  
    // Encourage user to rate after scrolling
    function setupScrollPopup() {
      let ratingPopupShown = false;
      window.addEventListener("scroll", () => {
        if (!ratingPopupShown && window.scrollY > 600) {
          alert("Enjoying the site? Please rate us at the bottom! ⭐");
          ratingPopupShown = true;
        }
      });
    }
  
    // Initialize all interactions on page load
    document.addEventListener("DOMContentLoaded", () => {
      setupRatings();
      setupScrollPopup();
    });
  </script>
  
  
</body>
</html>
