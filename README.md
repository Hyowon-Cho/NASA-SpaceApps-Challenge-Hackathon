# NASA SpaceApps Challenge 2024
## Team Groudon Detector 🌍

## Objectives
Detecting seismic activity on Mars and the Moon is essential for understanding planetary geology and enhancing space exploration. Our goal is to develop a model to identify seismic anomalies in planetary data to identify earthquakes. We also want to determine the patterns of seismicity on the Moon and Mars that we hypothesize can be divided into foreshocks, mainshocks, and aftershocks similar to Earth.

## Steps
### Step 1 🌘
For **Lunar data**, the data is relatively sufficient than Mars. For **Mars data**, we used IQR Method to overcome the problem of insufficient data. We trained scalar function to scale the datasets before we put them into our model.

### Step 2 🌗
We used **LSTM Autoencoder** to detect anomalies in time series data.

### Step 3 🌖
We visualized the detected anomalies in a graph, and highlighted the anomalies with a red marker for analysis.

### Step 4 🌕
We outputted the **CSV files** from the data that detected anomalies on the graph.

## Research Results

### Pattern Analysis 🌍
* Our analysis revealed patterns in lunar and Martian seismic activities that appear to follow Earth-like sequences of foreshocks, mainshocks, and aftershocks
* The detected patterns, while similar in sequence, showed unique characteristics specific to each celestial body

### Lunar Seismic Characteristics 🌘
#### Data Analysis
* Benefited from relatively sufficient data compared to Mars
* Successfully applied LSTM Autoencoder without requiring additional data processing techniques
* Clear pattern recognition achieved through comprehensive dataset

#### Detection Results
* Multiple seismic sequences identified through anomaly detection
* Reconstruction MAE showed expected right-skewed distribution
* Threshold determination proved effective for identifying significant events

### Martian Seismic Analysis 🌓
#### Data Processing
* Successfully implemented IQR method to address data insufficiency
* Maintained data integrity while generating usable training sets
* Scaled datasets effectively before model implementation

#### Key Findings
* Plot 1 demonstrated a medium-intensity precursor, followed by a major event and smaller subsequent activity
* Plot 2 revealed a sequence of three minor events preceding a major seismic event, followed by continued vibrations
* Pattern consistency suggests reliable detection despite limited data

## Conclusions and Future Directions 🎓

### Research Impact
#### Methodological Achievements
* Successfully developed and implemented LSTM Autoencoder for planetary seismic detection
* Created an effective framework for analyzing limited datasets through IQR method
* Established reliable threshold determination process for anomaly detection

#### Scientific Discoveries
* Confirmed the presence of three-phase seismic patterns on other planetary bodies
* Demonstrated the effectiveness of machine learning in extraterrestrial seismic detection
* Identified unique characteristics of planetary seismic events

### Future Research Opportunities
#### Technical Improvements
* Expand training dataset size beyond hackathon limitations
* Enhance model performance through extended testing periods
* Develop more sophisticated pattern recognition algorithms

#### Scientific Extensions
* Further investigation of detected patterns across longer time periods
* Comparative analysis of seismic characteristics between Earth, Moon, and Mars
* Integration with other planetary data sources

### Final Remarks
* Despite time constraints of the NASA Space Apps Challenge, we successfully developed a functional seismic detection algorithm
* Our findings suggest promising applications for planetary exploration and geological understanding
* The methodology provides a foundation for future research in extraterrestrial seismic activity detection

