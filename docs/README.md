<div align="center">
    <h1>Maxis E-Invoice Portal</h1>
</div>

### What is an e-Invoice?
An e-Invoice is a digital representation of a transaction between a seller and a buyer. e-Invoice is intended to replace paper or electronic documents of invoices, credit notes, debit notes and refund notes and contains the same essential transactional data. For more information, refer to LHDN e-Invoice microsite at e-Invoice | Lembaga Hasil Dalam Negeri Malaysia.


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
    width: 100px;
    height: 100px; 
    object-fit: contain; 
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
    { title: 'Authentication', logo: '../_media/readme/authentication.svg', link: '#/_authentication' },
    { title: 'Dashboard', logo: '../_media/readme/dashboard.svg', link: '#/_dashboard' },
    { title: 'Submission Details', logo: '../_media/readme/submissionDetails.svg', link: '#/_submission_details' },
    { title: 'Validate Tin', logo: '../_media/readme/validateTin.svg', link: '#/_validate_tin' },
    { title: 'Submission From BQ', logo: '../_media/readme/submissionFromBQ.svg', link: '#/_submission_from_bq' },
    { title: 'Settings', logo: '../_media/readme/settings.svg', link: '#/_settings' }
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