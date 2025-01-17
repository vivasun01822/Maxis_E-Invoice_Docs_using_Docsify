<div align="center">
    <h1>Maxis E-Invoice Portal</h1>
</div>

<div align="center" style="margin-top: 10%;">
    <h2>Features</h2>
</div>

<style>
  .grid-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
    gap: 20px;
    margin-top: 20px;
    padding: 0 20px;
  }
  .grid-item {
    background-color: #ffffff;
    border: 1px solid #e0e0e0;
    border-radius: 12px;
    padding: 20px;
    text-align: center;
    transition: transform 0.3s, box-shadow 0.3s;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  .grid-item:hover {
    transform: translateY(-10px);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
  }
  .grid-item img {
    max-width: 80px;
    margin-bottom: 15px;
  }
  .grid-item h3 {
    margin: 15px 0;
    font-size: 1.4em;
    color: #333;
  }
</style>

<div class="grid-container" id="features-grid"></div>

<script>
  const features = [
    { title: 'Authentication', logo: '../_media/logo1.png', link: '#/_authentication' },
    { title: 'Dashboard', logo: '../_media/logo2.png', link: '#/_dashboard' },
    { title: 'Submission Details', logo: '../_media/logo3.png', link: '#/_submission_details' },
    { title: 'Validate Tin', logo: '../_media/logo4.png', link: '#/_validate_tin' },
    { title: 'Submission From BQ', logo: '../_media/logo5.png', link: '#/_submission_from_bq' },
    { title: 'Settings', logo: '../_media/logo6.png', link: '#/_settings' }
  ];

  const gridContainer = document.getElementById('features-grid');

  features.forEach(feature => {
    const gridItem = document.createElement('a');
    gridItem.href = feature.link;
    gridItem.className = 'grid-item';
    gridItem.innerHTML = `
      <img src="${feature.logo}" alt="${feature.title} Logo">
      <h3>${feature.title}</h3>
    `;
    gridContainer.appendChild(gridItem);
  });
</script>