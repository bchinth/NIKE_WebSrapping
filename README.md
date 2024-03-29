# NIKE_WebSrapping
Nike Unisex Footwear Trends: A Web Scraping Data Analysis


In an advanced analysis initiative, our team utilized sophisticated web scraping techniques to collect and categorize data on Nike's unisex footwear into sale and non-sale segments. Utilizing a structured MySQL database, we applied meticulous data manipulation, wrangling and modeling to craft a high-quality dataset. This dataset then served as the foundation for a Machine Learning (ML) project aimed at uncovering common themes within Nike product descriptions through an unsupervised ML model that emphasized frequency over sequence. Our analysis revealed key themes that are crucial for enhancing Nike's marketing and product development strategies. This data-driven approach not only provides valuable insights into Nike's product positioning but also pioneers the use of analytics in retail strategy optimization.
BACKGROUND
In the fast-paced and highly competitive athletic footwear market, understanding customer preferences and market trends is paramount for a leading brand like Nike. The brand is renowned for its vast range of unisex shoes, catering to a wide spectrum of sports and lifestyle choices. Keeping abreast of market demands and ensuring the alignment of product offerings with consumer expectations is a critical business imperative . That's the reason why we choose to select an e-commerce website to delve deeper and understand the trends


CONTEXT
To stay at the forefront of the industry, our team has implemented a data-driven approach to understand Nike's market positioning better. We systematically collected detailed product data from Nike's online catalog, specifically focusing on the unisex footwear category. This data spans both sale and non-sale items, capturing nuances in pricing, product descriptions, reviews,
1
 ratings, and more. The extracted data was then meticulously processed and organized within a MySQL database, forming the basis for in-depth analysis.

 
DOMAIN KNOWLEDGE
The athletic footwear industry is characterized by fierce competition and swift changes in consumer trends. Products are not only designed for performance but also as fashion statements, requiring a fragile balance between functionality and aesthetic appeal. The branding and marketing of such products must resonate with diverse consumer bases, making the understanding of underlying themes in product descriptions vital for crafting compelling marketing narratives.
Nike, being a household name, holds an extensive collection that goes beyond mere footwear, encompassing a lifestyle. With product lines named after athletes, technologies developed for performance enhancement, and sustainability becoming increasingly important, the company's portfolio reflects a commitment to innovation and social responsibility.


INTRODUCTION TO DATA
Data Sources:
Nike's official online retail store - Nike's official site
The data source is Nike's sales and non-sale webpage, showcasing unisex shoes with and without discounts. It includes a variety of athletic and lifestyle footwear, displaying sale prices, discounts, and product images. This page is ideal for scraping sales trends and pricing data, allows for filtering by categories such as gender and sport, offering insights into consumer preferences and pricing strategies.


WEB SCRAPING ROUTINE(S)
Our web scraping routine targets Nike’s unisex shoe sales, structured into distinct stages: initialization, data extraction, content saving, and subsequent parsing. Initiated with Selenium, the process navigates Nike’s website, interacts with specific web elements to filter and sort products, and employs infinite scrolling to ensure full page content is loaded. The page source is then saved as a local HTML file. This file is parsed using BeautifulSoup to extract detailed product data. The extracted information is ready for further analysis or database storage.

The automation process involves a scripted sequence executed through the Selenium WebDriver. Initially, required Selenium modules are imported to facilitate browser interaction. Then, a Chrome WebDriver instance is initiated, which waits up to 10 seconds for page elements to load. The automated browser navigates to Nike's website, where it sequentially clicks through the site’s categories to reach the unisex shoes on sale. To accommodate web pages with lazy loading, an infinite scroll is implemented, ensuring all products are fully loaded for data capture. The same is repeated for the shoes not on sale under the unisex category again. This process sets up the stage for a comprehensive scrape of product listings.

