# Beer Project Analysis 🍺🔬

---

## 📌 Project Summary

This project performs a comprehensive data analysis of beer reviews and ratings to identify the characteristics of popular and high-quality beers. The goal is to provide data-driven insights to local Spanish breweries, helping them to create a beer with features that are likely to be successful in the market. The analysis focused on the correlation between review features, with **Taste** and **Palate** identified as key indicators. The study found that popular beers share characteristics such as being **dark**, **bitter**, and **strong**, with a **different** and distinct character. This project demonstrates the power of using data analysis to inform business strategy in the brewing industry.

---

## 📊 Dataset Overview

Data source: [https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate](https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate)
Other data sources: `beeradvocate.com`, `craftbeer.com`, `untapped.com`, `damm.com`, `corporacionhijosderivera.com`, `heinekenespana.es`, `mahou-sanmiguel.com`, `ccc.es`

The project utilizes four datasets for analysis:

### 📥 Input Features:

- **Main Dataset**:
  - **Source**: Kaggle
  - **Size**: 1.5 million entries, 14 columns
  - **Features**: `review_overall`, `review_aroma`, `review_appearance`, `style_id`, `review_palate`, `review_taste`, `year`

- **Craftbeer.com Dataset**:
  - **Source**: `craftbeer.com` (scraped)
  - **Size**: 72 entries, 5 columns
  - **Features**: `style_id`, `votes`, `review_overall`, `year`, `local_review`

- **Beeradvocate.com & Untapped.com Dataset**:
  - **Source**: `beeradvocate.com` and `untapped.com` (scraped)
  - **Size**: 448 entries, 5 columns
  - **Features**: `beer_style`, `color`, `bitterness`, `alcohol`, `style_id`

- **SQL Database**:
  - A database was created with an ERM and ERD to structure the data, though the primary analysis was done using Python and Power BI.

---

## 🧠 Data Analysis Workflow

1.  **Data Scraping**:
    -   Web scraping was performed on `beeradvocate.com`, `craftbeer.com`, and `untapped.com` to collect additional reviews and beer characteristics.

2.  **Database Creation**:
    -   An SQL database was created to house the datasets, following a defined Entity-Relationship Model (ERM) and Entity-Relationship Diagram (ERD).

3.  **Data Analysis**:
    -   Analysis was primarily conducted using Python and Power BI.
    -   **Pearson's correlation coefficient** was used to determine the relationships between the four review features (`taste`, `palate`, `aroma`, `appearance`).
    -   **Taste** was identified as having a higher correlation score with the overall review than any other feature.
    -   The analysis identified key popular beer characteristics as being **dark**, **bitter**, **strong**, and having a **distinct** flavor profile.

---

## ✅ Requirements

-   Python
-   Power BI
-   SQL
-   `pandas`, `numpy`
-   `matplotlib.pyplot`, `seaborn`
-   `scipy.stats`
-   `requests`, `BeautifulSoup`, `datetime`, `time`

---

## 🚀 Future Enhancements:

-   Conduct an analysis on why the Equilater beer failed in the Spanish market.
-   Compare the success of Equilater with the success of microbreweries in the Basque country that have **Stout** beers as their flagship.

---

## 🔗 Links:

-   **Presentation**: [https://docs.google.com/presentation/d/1ozVUopCIDAPglg9pb36o5dE_mnNvA9vefSYyn9z2y2M/edit?slide=id.g54dda1946d_6_332#slide=id.g54dda1946d_6_344](https://docs.google.com/presentation/d/1ozVUopCIDAPglg9pb36o5dE_mnNvA9vefSYyn9z2y2M/edit?slide=id.g54dda1946d_6_332#slide=id.g54dda1946d_6_344)
-   **Kaggle Dataset**: [https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate](https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate)
-   **Other Data Links**: `beeradvocate.com`, `craftbeer.com`, `untapped.com`, `damm.com`, `corporacionhijosderivera.com`, `heinekenespana.es`, `mahou-sanmiguel.com`, `ccc.es`