## Project Proposal

This project investigates the application of machine learning techniques to classify emotions from speech audio using the CREMA-D (Crowd-Sourced Emotional Multimodal Actors Dataset). The study focuses on distinguishing four primary emotions; happy, sad, angry, and fear, through acoustic feature analysis and explores how emotional intensity affects classification performance. By combining traditional feature engineering with ensemble learning methods, this research aims to develop robust emotion recognition models while examining the relationship between speech intensity and model confidence.

The project addresses two fundamental questions in acoustic emotion recognition: first, whether traditional machine learning algorithms can accurately classify emotions using engineered audio features, and second, how ensemble methods can significantly improve classification performance compared to individual models. This investigation contributes to the growing field of effective computing while demonstrating practical applications of ensemble learning principles in speech emotion recognition.

## Dataset Description

**Primary Dataset: CREMA-D (Crowd-Sourced Emotional Multimodal Actors Dataset)** **Provenance:** CREMA-D is a validated multi modal database created through collaboration between researchers and crowd sourced validation. The dataset contains emotional speech recordings from professional actors, making it ideal for supervised learning approaches to emotion classification.

### Dimensions & Structure:

| **Attribute** | **Details** |
|-------------------------|------------------------------------------------|
| **Total Files** | 7,442 audio clips from diverse emotional expressions |
| **Speakers** | 91 professional actors (48 male, 43 female) |
| **Age Range** | 20–74 years, providing demographic diversity |
| **Target Emotions** | 4 emotions selected for analysis (happy, sad, angry, fear) |
| **Emotional Intensities** | Multiple intensity levels (low, medium, high, unspecified) |
| **File Format** | WAV files suitable for feature extraction |
| **Sentence Variety** | 12 different sentences to reduce linguistic bias |

**Dataset Selection Rationale:** CREMA-D was chosen for its substantial size, demographic diversity, and established use in emotion recognition research. The dataset's systematic organization and intensity labels directly support both research questions, while its availability through Kaggle ensures reproducible research practices.

## Research Questions

### Question 1: Basic Emotion Classification

**Can we accurately classify four emotions (happy, sad, angry, fear) from audio features using traditional machine learning algorithms?**<br> This question investigates the fundamental capability of machine learning models to distinguish emotional states through acoustic analysis. By focusing on four distinct emotions, the study maintains sufficient complexity while ensuring manageable scope for comprehensive analysis.

### Question 2: Ensemble Learning Effectiveness

**Can combining multiple machine learning algorithms (ensemble methods) significantly improve emotion classification accuracy compared to individual models, and which ensemble strategies work best for acoustic emotion recognition?**<br> This question explores the relationship between emotional expression intensity and model performance, investigating whether stronger emotional expressions are easier to classify and whether audio features can predict when models will be confident in their predictions.


## Technical Implementation

**Programming Environment:** Python with scientific computing stack

#### Key Libraries

| **Library**              | **Purpose**                                 |
|--------------------------|---------------------------------------------|
| `librosa`                | Audio feature extraction and processing     |
| `scikit-learn`           | Machine learning algorithms and evaluation  |
| `pandas` / `numpy`       | Data manipulation and numerical computation |
| `matplotlib` / `seaborn` | Visualization and results presentation      |

## Expected Project Timeline (3\~ weeks)

#### Week 0: Data preparation and exploration

-   Download CREMA-D from Kaggle (\~2GB)
-   Explore dataset structure and file naming
-   Proposal write-up and review

#### Week 1: Feature extraction and dataset creation

-   Implement feature extraction pipeline
-   Process selected audio files
-   Create clean feature dataset
-   Exploratory data analysis of features vs emotions

#### Week 2: Individual model development

-   Train baseline models (Logistic Regression, Decision Tree, SVM)
-   Hyperparameter tuning using GridSearchCV
-   Performance evaluation and comparison
-   Feature importance analysis

#### Week 3: Ensemble methods and final analysis

-   Implement ensemble approaches
-   Compare individual vs ensemble performance
-   Statistical significance testing
-   Final report and presentation

## Project Structure

| Folder / File Name | Description |
|---------------------------------------------|---------------------------|
| `.quarto/` | Quarto's internal folder—automatically created to manage rendering settings and cache. You typically don't touch this. |
| `_freeze/` | Keeps locked-in versions of documents to ensure consistency when rebuilding or sharing. |
| `data/` | Where all the data lives—raw inputs, cleaned datasets, and a README explaining structure and sources. |
| `images/` | Used for storing visual content like charts, graphs, and illustrations referenced in your `.qmd` files. |
| `index.qmd` | Acts as the homepage, giving a snapshot of what the project is about. |
| `about.qmd` | Gives extra context—background info, author bio, or detailed project narrative. |
| `proposal.qmd` | The full research plan: includes goals, methods, schedule, and how everything is structured. |
| `presentation.qmd` | Slide deck made with Quarto to highlight the most important insights from your project. |

##
