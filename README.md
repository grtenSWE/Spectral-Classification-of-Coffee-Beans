Spectral Classification of Coffee Beans

This project applies Principal Component Analysis (PCA) to FTIR (Fourier Transform Infrared) reflectance spectra of Arabica and Robusta coffee beans to identify key wavelength features and classify samples based on their spectral signatures.

Overview

The goal is to explore how dimensionality reduction and feature extraction can reveal class-separating patterns in high-dimensional spectral data. Using PCA, the dominant wavelength regions responsible for most of the spectral variance are identified and used for classification.

Methods
	•	Data Preprocessing: Loaded and normalised FTIR reflectance spectra; centered data and computed covariance matrices over wavenumbers (cm⁻¹).
	•	PCA Analysis: Performed eigen-decomposition to extract principal components; visualised scree and cumulative variance plots.
	•	Classification: Built a pipeline using PCA + L1-regularised logistic regression; tuned the regularisation parameter with golden-section search and cross-validation.
	•	Reconstruction: Reconstructed spectra from leading PCs to evaluate low-dimensional representation fidelity.

Results
	•	Achieved 95% classification accuracy distinguishing Arabica and Robusta beans.
	•	Identified key wavelength regions contributing to inter-class spectral differences.
	•	Demonstrated that the first six principal components capture over 98% of total variance.

Tech Stack
	•	Languages: Python
	•	Libraries: NumPy, Pandas, scikit-learn, Matplotlib
	•	Techniques: PCA, eigen-decomposition, logistic regression, cross-validation

Author

Andy Tran
BEng(Hons)/BSc – Engineering Science & Computer Science
University of Auckland
linkedin.com/in/andyuoa
