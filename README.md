🌊 Fisheries Growth and Ocean Plastic Accumulation Analysis
   
Investigating the relationship between global fisheries expansion and oceanic plastic pollution using time-series forecasting and predictive modeling

📊 Key Findings
840% increase in global fisheries production from 1950 to 2020
300-400% increase in oceanic microplastic concentrations over the same period
Strong positive correlation (r = 0.82, p < 0.001) between fisheries growth and plastic accumulation
ARIMA forecasts suggest plastic pollution may increase faster than fisheries output through 2050
Evidence of a positive feedback loop between fishing activity and marine plastic pollution

🎯 Project Overview
This research investigates two interconnected environmental trends: the growth of the global fishing industry and the accumulation of plastic waste in the world's oceans. Using 70 years of historical data (1950-2020), we apply statistical analysis, correlation studies, and ARIMA time-series forecasting to:
Quantify long-term trends in fisheries production and ocean plastics
Assess the strength of relationships between these variables
Project future trajectories for both fisheries and plastic pollution
Explore environmental implications and policy recommendations
Research Questions
How have global fisheries production and ocean plastic pollution changed over the past 70 years?
Is there a statistical relationship between fisheries expansion and plastic accumulation?
What do current trends suggest about future environmental impacts?
What interventions could break the positive feedback loop?

📸 Visual Preview
Correlation Between Fisheries and Microplastics
 Strong positive correlation (r = 0.82) between fisheries production and microplastic concentration
ARIMA Forecasts Through 2050
 Time-series projections showing accelerating plastic accumulation relative to fisheries growth

🗂️ Repository Structure
fisheries-ocean-plastics-analysis/
│
├── data/                      # Raw and processed datasets
│   ├── raw/                   # Original data from FAO, NOAA
│   └── processed/             # Cleaned, analysis-ready data
│
├── notebooks/                 # Jupyter notebooks (analysis workflow)
│   ├── 01_data_exploration.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_correlation_analysis.ipynb
│   ├── 04_arima_modeling.ipynb
│   └── 05_visualization.ipynb
│
├── src/                       # Python source code (reusable modules)
│   ├── data_processing.py
│   ├── statistical_analysis.py
│   ├── time_series_models.py
│   └── visualization.py
│
├── scripts/                   # Standalone execution scripts
│   ├── run_full_analysis.py
│   └── generate_figures.py
│
├── figures/                   # All visualizations from the paper
│
├── results/                   # Model outputs and statistics
│
├── paper/                     # Research paper (PDF and Markdown)
│
└── docs/                      # Additional documentation


🚀 Getting Started
Prerequisites
Python 3.10 or higher
Jupyter Notebook or JupyterLab
Git (for cloning the repository)
Installation
Clone the repository

 git clone https://github.com/YOUR_USERNAME/fisheries-ocean-plastics-analysis.git
cd fisheries-ocean-plastics-analysis


Create a virtual environment (recommended)

 python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


Install dependencies

 pip install -r requirements.txt


Launch Jupyter Notebook

 jupyter notebook


Run notebooks in order (01 → 05)



📊 Data Sources
Primary Datasets
Global Fisheries Production (1950-2022)


Source: Food and Agriculture Organization (FAO)
Variables: Total capture production (million tonnes), Year
Coverage: Annual global data
Microplastic Concentrations (1972-2022)


Source: NOAA Marine Debris Program
Variables: Sample counts, Mean concentration (particles/m³), Year
Coverage: Aggregated oceanographic measurements
Great Pacific Garbage Patch Data


Source: The Ocean Cleanup
Variables: Plastic composition, Mass estimates
Used for contextual analysis
Note: Due to file size, raw data is not included in this repository. Run scripts/download_data.py to fetch data from sources, or access processed data in data/processed/.

🔬 Methodology
Statistical Analysis
Correlation Analysis: Pearson correlation coefficient with significance testing
Time Series Analysis: Stationarity tests (Augmented Dickey-Fuller)
Regression Analysis: Linear and polynomial models
Predictive Modeling
ARIMA(2,1,2) models for both fisheries and plastics
Model selection via ACF/PACF diagnostics
30-year forecasts (2021-2050) with confidence intervals
Performance metrics: RMSE, MAE, AIC, BIC
Tools & Libraries
Data Processing: pandas, NumPy
Statistical Analysis: statsmodels, SciPy
Modeling: statsmodels.tsa.arima
Visualization: Matplotlib, Seaborn
Environment: Python 3.10, Google Colab
See docs/methodology.md for detailed technical documentation.

📈 Key Results
Historical Trends (1950-2020)
Fisheries production: 19 → 179 million tonnes (+840%)
Microplastic concentration: ~10 → 40-50 particles/m³ (+300-400%)
Peak growth periods coincide: 1970s-1980s for both variables
Statistical Relationships
Pearson r = 0.82 (p < 0.001) between fisheries and plastics
R² = 0.67: 67% shared variance
Granger causality test suggests temporal precedence from fisheries to plastics
ARIMA Forecasts (2050 Projections)
Fisheries: ~115 million tonnes (95% CI: [98, 132])
Microplastics: ~145 particles/m³ (95% CI: [110, 180])
Key Finding: Plastic accumulation rate exceeds fisheries growth rate
Model Performance
Fisheries model: RMSE = 4.2 MT, MAE = 3.1 MT
Plastics model: RMSE = 8.7 p/m³, MAE = 6.3 p/m³

🌍 Environmental Implications
Positive Feedback Loop Identified
Fisheries expansion → Increased gear loss and supply chain waste
Plastic accumulation → Marine habitat degradation
Ecosystem damage → Reduced fish stock resilience
Intensified fishing → More pressure on remaining stocks → Return to step 1
Policy Recommendations
Gear Tracking Systems: Mandatory RFID/GPS tracking for fishing equipment
Material Innovation: Accelerate biodegradable gear research and adoption
Recovery Programs: Incentivize gear retrieval through bounty systems
Circular Economy: Implement take-back and recycling schemes at ports
Enhanced Monitoring: Expand standardized microplastic sampling globally
Regional Analysis: Identify hotspots for targeted interventions
International Cooperation: Strengthen transboundary agreements on marine debris

📄 Research Paper
The full research paper is available in the paper/ directory:
PDF: Research_Paper_Final.pdf
Markdown: Research_Paper_Final.md
Abstract: This study investigates the connection between the expanding global fishing industry and the accumulation of ocean plastics using 70 years of historical data. Results reveal an 840% increase in fisheries production and 300-400% increase in microplastic concentrations between 1950 and 2020, with strong positive correlation (r = 0.82, p < 0.001). ARIMA forecasts suggest plastic pollution may outpace fisheries growth through 2050, highlighting the need for sustainable management interventions.

🔄 Reproducibility
This project prioritizes reproducibility:
✅ Complete code and notebooks: All analysis steps documented
 ✅ Dependency management: requirements.txt with pinned versions
 ✅ Data documentation: Sources, collection methods, preprocessing steps
 ✅ Model specifications: Full ARIMA parameters and diagnostics
 ✅ Version control: Git history shows analysis evolution
To reproduce results:
Clone repository
Install dependencies (pip install -r requirements.txt)
Download data (python scripts/download_data.py)
Run notebooks sequentially (01 → 05)
Or run complete pipeline: python scripts/run_full_analysis.py

📊 Figures
All figures from the research paper are available in high resolution:
Figure
Description
File
1
Number of Samples Per Year
figure_01_samples_per_year.png
2
Total Fisheries Production by Year
figure_02_fisheries_production.png
3
Data Availability by Year
figure_03_data_availability.png
4a
Global Fisheries Production (1950-2022)
figure_04a_fisheries_temporal.png
4b
Microplastic Concentration (1972-2022)
figure_04b_plastics_temporal.png
5a
Fisheries vs Microplastic Concentration
figure_05a_scatter_plot.png
5b
Correlation Matrix
figure_05b_correlation_matrix.png
6a
Distribution of Fisheries Production
figure_06a_fisheries_distribution.png
6b
Distribution of Microplastic Concentration
figure_06b_plastics_distribution.png
7
ACF and PACF Plots
figure_07_acf_pacf_plots.png
8a
ARIMA Forecast: Fisheries Production
figure_08a_fisheries_forecast.png
8b
ARIMA Forecast: Microplastic Concentration
figure_08b_plastics_forecast.png


🤝 Contributing
Contributions are welcome! Ways to contribute:
Report bugs: Open an issue describing the problem
Suggest enhancements: Propose new analyses or visualizations
Improve documentation: Fix typos, add examples, clarify instructions
Add features: Submit pull requests with new functionality
Contribution Workflow
# Fork the repository
# Clone your fork
git clone https://github.com/YOUR_USERNAME/fisheries-ocean-plastics-analysis.git

# Create a branch
git checkout -b feature/your-feature-name

# Make changes and commit
git commit -m "Add your descriptive commit message"

# Push to your fork
git push origin feature/your-feature-name

# Open a Pull Request on GitHub


📜 Citation
If you use this code, data, or findings in your research, please cite:
@misc{fisheries_plastics_2026,
  author = {[Your Name]},
  title = {Assessing the Relationship Between Global Fisheries Growth and 
           Oceanic Plastic Accumulation Using Predictive Modelling Techniques},
  year = {2026},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/YOUR_USERNAME/fisheries-ocean-plastics-analysis}},
  doi = {[DOI pending]}
}

APA Format:
 [Your Name]. (2026). Assessing the Relationship Between Global Fisheries Growth and Oceanic Plastic Accumulation Using Predictive Modelling Techniques. GitHub. https://github.com/YOUR_USERNAME/fisheries-ocean-plastics-analysis

📧 Contact
Author: [Your Name]
 Institution: [Your School/University]
 Email: [your.email@example.com]
 LinkedIn: [Your LinkedIn Profile]
 Website: [Your Website] (optional)
For questions about the research, methodology, or code:
Open an Issue
Email directly: [your.email@example.com]

🙏 Acknowledgments
Data Sources: FAO, NOAA, The Ocean Cleanup for providing open data
Mentors: [Mentor names] at Ascend Now for guidance and support
Libraries: The Python data science community for excellent tools
References: All cited researchers whose work informed this study
Special thanks to the marine conservation community working to protect our oceans.

📋 License
This project is licensed under the MIT License - see the LICENSE file for details.
Summary: You are free to use, modify, and distribute this code with attribution. No warranty is provided.

🔗 Additional Resources
Related Research
Ocean Cleanup Research
FAO Fisheries Statistics
NOAA Marine Debris Program
Learning Resources
Time Series Analysis in Python
Environmental Data Science
Marine Pollution Research
Tools & Libraries Documentation
pandas
statsmodels
matplotlib
seaborn

📊 Project Status
Current Status: ✅ Active - Research Complete, Code Published
Latest Updates:
February 2026: Initial publication
Paper finalized with peer review
All code and data documentation complete
Future Plans:
Regional analysis by ocean basin
Machine learning models for comparison
Real-time monitoring dashboard
Policy impact assessment

⭐ Star This Repository
If you find this research useful, please consider starring ⭐ the repository to help others discover it!
 <div align="center">
🌊 Protecting Our Oceans Through Data-Driven Research 🌊
Made with 💙 for marine conservation
</div>
