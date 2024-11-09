# **SponsorSpotter 2.0**

SponsorSpotter 2.0 is an AI-powered, cloud-based platform designed to streamline the sponsorship decision-making process. By analyzing YouTube channel metrics, sentiment, and content alignment, the platform helps sponsors find optimal YouTube channels for their products. The system leverages Vultr’s cloud infrastructure for efficient data storage, retrieval, and analysis, ensuring scalability and high performance.

---

## **Index**

1. [Project Overview](#project-overview)
2. [Objectives](#objectives)
3. [Methodology](#methodology)
   - [Content and Product Alignment Analysis](#content-and-product-alignment-analysis)
   - [Audience Sentiment Analysis](#audience-sentiment-analysis)
   - [Likes-to-Views Ratio Assessment](#likes-to-views-ratio-assessment)
   - [Subscriber Count Evaluation](#subscriber-count-evaluation)
   - [Channel View Count Analysis](#channel-view-count-analysis)
   - [Final Evaluation](#final-evaluation)
4. [Installation and Setup](#installation-and-setup)
5. [Directory Structure](#directory-structure)
6. [Contributing](#contributing)
7. [Acknowledgments](#acknowledgments)

---

## **Project Overview**

SponsorSpotter 2.0 helps brands optimize their influencer marketing efforts by recommending YouTube channels best suited for sponsorship. It combines AI, Machine Learning, and NLP to analyze content alignment, sentiment, engagement, and growth metrics, providing data-driven insights for sponsorship decisions. With the support of Vultr’s cloud infrastructure, the platform can scale as data grows and deliver real-time recommendations.

---

## **Objectives**

- **Data Collection**: Efficiently gather YouTube channel metrics, including views, likes, and engagement stats.
- **Content Alignment**: Use GloVe encoding to compare sponsor product descriptions with YouTuber content.
- **Audience Sentiment Analysis**: Utilize NLP to evaluate comments and determine audience engagement.
- **Growth and Engagement Analysis**: Assess likes-to-views ratios, subscriber count, and total views to rank YouTube channels.
- **Sponsorship Recommendations**: Develop a system that ranks channels based on various factors and recommends the best options for sponsorship.

---

## **Methodology**

### **1. Content and Product Alignment Analysis**
- Retrieve YouTube channel content and sponsor product descriptions.
- Apply GloVe encoding for vectorizing both content and product descriptions.
- Calculate cosine similarity to measure content-product alignment.

### **2. Audience Sentiment Analysis**
- Use the YouTube API to collect comments from target channels.
- Apply NLP techniques (TextBlob) to analyze sentiment and engagement levels.
- Calculate the ratio of positive, negative, and neutral sentiments.

### **3. Likes-to-Views Ratio Assessment**
- Measure the ratio of likes to views across all videos for each channel to gauge audience interaction and quality.

### **4. Subscriber Count Evaluation**
- Analyze the channel’s subscriber count and growth patterns to evaluate the channel’s overall reach and stability.

### **5. Channel View Count Analysis**
- Track total views to assess the channel’s popularity and audience size.

### **Final Evaluation**
- Normalize each parameter for a fair comparison.
- Aggregate scores from all metrics and determine the best channel for sponsorship.
- Provide a final ranking and recommendation based on the calculated score.

---

## **Installation and Setup**

### **1. Clone the Repository**
```bash
git clone https://github.com/yourusername/SponsorSpotter2.0.git
cd SponsorSpotter2.0
```

### **2. Install Dependencies**
Make sure you have Python 3.x installed. Then, install the required packages:
```bash
pip install -r requirements.txt
```

### **3. API Keys**
- Obtain YouTube API keys and update the configuration file with your keys.

### **4. Run the Application**
```bash
python app.py
```

The web application will be hosted at `http://localhost:5000`.

---

## **Directory Structure**

```
SponsorSpotter2.0/
│
├── static/                 # Static assets (images, CSS)
│   └── images/             # Image files
│
├── templates/              # HTML templates for rendering views
│   ├── index.html
│   ├── login.html
│   ├── profile.html
│   ├── result.html
│   └── signup.html
│
├── app.py                  # Flask app
└── requirements.txt        # List of dependencies
```

---

## **Contributing**

1. **Fork the repository**.
2. **Create a feature branch**:
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Commit your changes**:
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. **Push to the branch**:
   ```bash
   git push origin feature/AmazingFeature
   ```
5. **Open a pull request**.

---

## **Acknowledgments**

- [YouTube API](https://developers.google.com/youtube/v3) for data collection.
- [GloVe: Global Vectors for Word Representation](https://nlp.stanford.edu/projects/glove/) for content and product alignment.
- [TextBlob](https://textblob.readthedocs.io/en/dev/) for sentiment analysis.
- [Vultr](https://www.vultr.com) for cloud storage and compute resources.

---
