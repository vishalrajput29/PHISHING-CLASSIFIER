
# Phishing Classification Using Machine Learning

This project focuses on building a machine learning model to classify URLs as either phishing or legitimate. Phishing attacks are a significant cybersecurity threat, where attackers deceive users by disguising malicious websites as trustworthy ones. The project involves data preprocessing, feature extraction, and the application of machine learning algorithms to detect phishing URLs. Additionally, a complete CI/CD pipeline has been implemented to ensure seamless integration, testing, and deployment of the model, facilitating continuous updates and improvements.


## Author

- [@vishalrajput](https://github.com/vishalrajput29/PHISHING-CLASSIFIER)


## Badges



[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)


## Project Lifecycle

![lifecycle](https://github.com/user-attachments/assets/49011b25-3eb6-4353-8f40-5d28c53eb34f)
## Run


To Create an Environment

```cmd
  conda create -p venv python==3.9 -y
```

To Run the Project

```cmd
  python app.py
```

To Run the reqiurement.txt file

```cmd
  pip install -r reqiurement.txt
```


## Data 

Paper Link : https://www.sciencedirect.com/science/article/pii/S2352340920313202

Dataset Link : https://data.mendeley.com/datasets/72ptz43s9v/1
## Technologies Used

Here’s a list of technologies you can include in your README file for the phishing classification machine learning project:

---

### Technologies Used

- **Python**: Core programming language for building and deploying the model.
- **Scikit-learn**: For machine learning model development and evaluation.
- **Pandas**: Data manipulation and preprocessing.
- **NumPy**: Numerical computations.
- **Flask**: For creating a lightweight web API to serve the model.
- **Docker**: Containerization of the application to ensure consistent environments across development, testing, and production.
- **GitHub Actions**: CI/CD tools for automating the pipeline, including testing and deployment.
- **Git**: Version control for tracking changes and collaboration.
- **AWS**: Cloud platform for deploying the application (S3 Bucket).


---

![OIP (1)](https://github.com/user-attachments/assets/c9eea634-f643-4d09-a4f6-596645f8d5f0)
## Data Description


1. **having_IP_Address**: Indicates whether the URL contains an IP address (Phishing URLs often use IP addresses instead of domain names).
  
2. **URL_Length**: The length of the URL. Longer URLs are sometimes used to deceive users.
  
3. **Shortining_Service**: Whether a URL shortening service is used (e.g., bit.ly).
  
4. **having_At_Symbol**: Checks for the presence of "@" symbol in the URL (used to redirect traffic).
  
5. **double_slash_redirecting**: Indicates if "//" appears after the domain (can be used to redirect to another site).
  
6. **Prefix_Suffix**: The presence of "-" in the domain, which can indicate a deceptive website.
  
7. **having_Sub_Domain**: The number of subdomains in the URL. More subdomains can indicate phishing attempts.
  
8. **SSLfinal_State**: Status of the SSL certificate. Legitimate sites typically have a valid SSL certificate.
  
9. **Domain_registeration_length**: The length of time the domain has been registered. Phishing sites often have short registration periods.
  
10. **Favicon**: Checks if the favicon is loaded from the main domain or a third party.
  
11. **port**: Whether non-standard ports are used (phishing sites sometimes use unusual ports).
  
12. **HTTPS_token**: If the URL contains "HTTPS" in the domain name to appear secure.
  
13. **Request_URL**: Checks if the external resources (like images) are loaded from the same domain or external sources.
  
14. **URL_of_Anchor**: Examines the anchor tags within the page; a high percentage of external links might indicate phishing.
  
15. **Links_in_tags**: Similar to the above, but for meta, script, and link tags.
  
16. **SFH (Server Form Handler)**: The server form handler field; empty or "about:blank" values are suspicious.
  
17. **Submitting_to_email**: Checks if the form data is submitted via email (phishing sites often use this).
  
18. **Abnormal_URL**: Indicates if the URL is considered abnormal or suspicious.
  
19. **Redirect**: The number of times the page has been redirected.
  
20. **on_mouseover**: Changes in the URL when the mouse is hovered over a link (common in phishing).
  
21. **RightClick**: Disabling the right-click function, which is often used to prevent inspection of the site.
  
22. **popUpWidnow**: Whether the page spawns popup windows, which can be used for phishing.
  
23. **Iframe**: The use of iframes to display content (phishing sites often use iframes to hide the original content).
  
24. **age_of_domain**: The age of the domain; phishing sites often have newly registered domains.
  
25. **DNSRecord**: DNS record status, which can indicate whether the domain is suspicious or not.
  
26. **web_traffic**: The amount of traffic the domain receives; phishing sites often have low traffic.
  
27. **Page_Rank**: The page rank of the site (phishing sites typically have a low rank).
  
28. **Google_Index**: Whether the site is indexed by Google (many phishing sites are not).
  
29. **Links_pointing_to_page**: The number of links pointing to the webpage (phishing sites often have fewer backlinks).
  
30. **Statistical_report**: Whether the site has been flagged in statistical phishing reports.
  
31. **Result**: The target variable, where `-1` indicates a phishing site, and `1` indicates a legitimate site.

## Screenshots

![predict](https://github.com/user-attachments/assets/3fd8d4b3-1857-4724-beb1-38fbd12d0628)

