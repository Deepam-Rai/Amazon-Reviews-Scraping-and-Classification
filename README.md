# **Amazon-Reviews-Scraping-and-Classification**
Scraping the reviews for a product at Amazon using Beautiful Soup and applying Machine Learning techniques to classify them as positive/negative reviews.  
This work was done as an assignment for ML course at SSSIHL.  

**Language Used:** Python
## **Scraping**  
Library Used: BeautifulSoup

## **Dataset**
**Amazon Product:** Reviews for Juarez Acoustic Guitar at amazon.in.  
**Link:** https://www.amazon.in/Juarez-Acoustic-Cutaway-038C-Strings/dp/B017NPCSLI/ref=cm_cr_arp_d_product_top?ie=UTF8  
Number of observations: 4423  
Columns: Review and corresponding stars given by the customer.  
1,2 and 3 star reviews are taken as Negative reviews and 4 and 5 stars as Positive reviews.  
Number of Positive reviews: 2887  
Number of Negative reviews: 1536  

## **Data Balancing:**
Random undersampling is performed to get 1536 data points of each class.  

## **Modelling**
Count Vectorizer is used to transform the reviews to machine readable format.  
**Train Test Split Ratio:** 80-20 train-test

**ML Techniques used:**  
1. **Gaussian Naive Bayes**
1. **Random Forest**
1. **Penalized SVM** (On imbalanced data)

## **Conclusion:**
From the classification report generated we find that **Penalized SVM** performs best.
