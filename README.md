# Crypto Clustering — K-Means + PCA on Market Data

Unsupervised learning on cryptocurrency 24h/7d/30d/... price-change features (`Crypto_Clustering.ipynb`): can market behavior cluster coins, and does dimensionality reduction sharpen the picture?

## Method
1. Normalize features with `StandardScaler`
2. **Elbow method** on the original feature space → best k = 4
3. K-means clustering, visualized on 24h vs 7d change
4. **PCA to three components**, explained variance computed (~89%)
5. Elbow + K-means re-run in PCA space; clusters compared side-by-side

## Takeaway
PCA preserved the cluster structure with fewer dimensions and produced tighter, more separable clusters — same k, less noise. The side-by-side plots make the case visually.

**Skills:** feature scaling, elbow analysis, K-means, PCA variance interpretation, hvplot.

---
*Built during the University of Texas Data Analysis Boot Camp (2023–24), with help from classmates, tutors, and AI tools — disclosed then, kept honest now.*
