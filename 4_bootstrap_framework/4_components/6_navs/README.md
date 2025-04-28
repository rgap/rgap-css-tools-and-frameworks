<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Bootstrap Tabs Example</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" />
  </head>
  <body>
    <div class="container mt-5">
      <h1 class="mb-4 text-center">Bootstrap Tabs</h1>

      <!-- Tabs Navigation -->
      <ul class="nav nav-tabs" id="myTab" role="tablist">
        <li class="nav-item" role="presentation">
          <button class="nav-link active" id="home-tab" data-bs-toggle="tab" data-bs-target="#home" type="button" role="tab" aria-controls="home" aria-selected="true">Home</button>
        </li>
        <li class="nav-item" role="presentation">
          <button class="nav-link" id="profile-tab" data-bs-toggle="tab" data-bs-target="#profile" type="button" role="tab" aria-controls="profile" aria-selected="false">Profile</button>
        </li>
        <li class="nav-item" role="presentation">
          <button class="nav-link" id="contact-tab" data-bs-toggle="tab" data-bs-target="#contact" type="button" role="tab" aria-controls="contact" aria-selected="false">Contact</button>
        </li>
      </ul>

      <!-- Tabs Content -->
      <div class="tab-content" id="myTabContent">
        <div class="tab-pane fade show active p-3" id="home" role="tabpanel" aria-labelledby="home-tab">
          Home tab content.
        </div>
        <div class="tab-pane fade p-3" id="profile" role="tabpanel" aria-labelledby="profile-tab">
          Profile tab content.
        </div>
        <div class="tab-pane fade p-3" id="contact" role="tabpanel" aria-labelledby="contact-tab">
          Contact tab content.
        </div>
      </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
  </body>
</html>