# CloudVandana
Assigment link of CloudVandana

1. Create a Simple Profile Card 
Design a responsive profile card using HTML and CSS. The card should include: 
• A profile picture 
• Name and designation 
• A short bio 
• Social media icons 
• The card should be centered on the page and adapt well to different screen sizes 
• Use CSS animations for a hover effect on the card.

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Profile Card</title>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
  <style>
    /* Global Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    /* Body Styling */
    
  body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #f4f4f4;
      margin: 0;
    }

    /* Profile Card Styling */
  .profile-card {
      background-color: #fff;
      width: 300px;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      overflow: hidden;
      transition: transform 0.3s ease;
    }

  .profile-card:hover {
      transform: translateY(-10px);
    }

    /* Profile Picture */
  .profile-card .profile-pic {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    /* Content Styling */
  .profile-card .content {
      padding: 20px;
      text-align: center;
    }

  .profile-card .content h2 {
      font-size: 22px;
      margin: 10px 0;
    }

  .profile-card .content p {
      font-size: 14px;
      color: #555;
      margin-bottom: 20px;
    }

  .profile-card .content .designation {
      font-weight: bold;
      color: #333;
    }

    /* Social Media Icons */
  .social-icons {
      display: flex;
      justify-content: center;
      gap: 15px;
    }

  .social-icons a {
      font-size: 18px;
      color: #555;
      transition: color 0.3s;
    }

  .social-icons a:hover {
      color: #007bff;
    }

    /* Responsive Design */
  @media (max-width: 480px) {
      .profile-card {
        width: 250px;
      }

  .profile-card .content h2 {
        font-size: 18px;
      }

  .profile-card .content p {
        font-size: 12px;
      }
    }
  </style>
</head>
<body>

  <div class="profile-card">
    <img src="https://via.placeholder.com/300x200" alt="Profile Picture" class="profile-pic">
    <div class="content">
      <h2>John Doe</h2>
      <p class="designation">Software Engineer</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam.</p>
      <div class="social-icons">
        <a href="#" class="fab fa-facebook-f"></a>
        <a href="#" class="fab fa-twitter"></a>
        <a href="#" class="fab fa-linkedin-in"></a>
        <a href="#" class="fab fa-github"></a>
      </div>
    </div>
  </div>

</body>
</html>
