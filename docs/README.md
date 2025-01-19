<div align="center" style="margin-bottom: 5%;">
    <h1>Maxis E-Invoice Portal</h1>
</div>

The Maxis E-Invoice Portal is a web-based application designed to simplify and streamline the process of managing e-invoices. It offers secure user authentication, a comprehensive dashboard, detailed submission logs, and TIN validation. The portal integrates with Google BigQuery for automated submissions and provides customizable settings for system preferences. Its responsive design ensures a seamless user experience across all devices.

<div align="center" style="margin-top: 5%;">
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

## Key Features and Functionalities:

### Authentication:

Ensures secure access to the portal by providing user authentication mechanisms.

### Dashboard:

Displays an overview of key metrics, activities, and summaries related to e-invoice management.
Helps users monitor the status of submissions and identify issues at a glance.

### Submission Details:
- Offers detailed logs of submitted e-invoices, including status, timestamps, and other relevant data.
- Allows users to track the lifecycle of each submission.

### Validate TIN:

Provides a mechanism to validate Taxpayer Identification Numbers (TIN) quickly and efficiently, ensuring compliance with regulatory standards.


### Submission From BigQuery:

- Integrates with Google BigQuery to facilitate automatic submission of e-invoices from pre-configured tables.
- Includes features to define triggers for real-time or scheduled submissions, minimizing manual intervention.

### Settings:

- Offers customizable options to configure system preferences, roles, and permissions.
- Enables administrators to manage key operational parameters of the portal.


### Audit Logs:

- Maintains a record of user activities and system operations, enabling administrators to monitor and trace actions for security and compliance purposes.
- Features search and filter options, such as by user email or date range, for precise tracking.


## User Experience:

### Responsive Design: 

The portal is designed to adapt seamlessly across devices, providing a consistent experience on desktops, tablets, and smartphones.

### User-Friendly Interface: 

Simplifies navigation and reduces learning curves with clear layouts and accessible options.

### Secure Operations: 
Implements role-based access control to ensure sensitive operations are restricted to authorized users.

### Benefits:
- **Efficiency:** Automates repetitive tasks, saving time and reducing human errors.
- **Compliance:** Ensures adherence to local and international standards for e-invoicing.
- **Scalability:** Integrates with BigQuery and supports large-scale operations for businesses handling extensive invoice data.