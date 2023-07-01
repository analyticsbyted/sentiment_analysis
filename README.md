# Fine Food Product Reviews Sentiment Analysis

This project focuses on sentiment analysis of customer reviews and star ratings for fine food products on Amazon.com. The goal is to analyze the sentiment expressed by customers in their reviews and correlate it with the star ratings.  NLTK and Hugging Face Transformers were employed to conduct the analysis.

## Dataset

The dataset used for this project consists of reviews of fine foods from Amazon. It spans a period of more than 10 years, including all ~500,000 reviews up to October 2012. The dataset includes product and user information, ratings, and plain text reviews from various Amazon categories.

### Contents

- `Reviews.csv`: This file contains the reviews data, pulled from the corresponding SQLite table named Reviews in `database.sqlite`.
- `database.sqlite`: This file contains the SQLite database, including the table 'Reviews'.

#### Data Overview

- Reviews from Oct 1999 - Oct 2012
- 568,454 reviews
- 256,059 users
- 74,258 products
- 260 users with > 50 reviews

### Dataset Sampling

To focus the analysis on a smaller subset of the dataset, we performed random sampling using the `sample_csv.ipynb` script included in this repository. The script randomly selects 500 reviews from the original `Reviews.csv` file and saves the sampled data as `sampled_data.csv`. This sampling was done to reduce the dataset size while still maintaining representative data.

## Citation

If you publish articles based on this dataset, please cite the following paper:

J. McAuley and J. Leskovec. From amateurs to connoisseurs: modeling the evolution of user expertise through online reviews. WWW, 2013.

## Installation

To run this project locally, please follow these steps:

1. Clone the repository to your local machine.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Ensure you have Python 3.6 or higher installed.
4. Download the `sampled_data.csv` file from the repository and place it in the project directory.
5. Run the Jupyter Notebook file `sentiment.ipynb` to perform sentiment analysis on the reviews.

## Usage

Once you have set up the project, you can use the Jupyter Notebook file `sentiment.ipynb` to perform sentiment analysis using VADER, Roberta, and Hugging Face transformers. The notebook provides step-by-step instructions and explanations on how to load the dataset, preprocess the data, and apply the sentiment analysis models.

## Results and Insights

The sentiment analysis results provide insights into the sentiment expressed by customers in their reviews. By correlating the sentiment with the star ratings, we can identify patterns and understand the relationship between customer sentiment and their ratings for fine food products. The project aims to uncover any interesting findings or trends in the data.

## Future Enhancements

There are several possible enhancements for this project:

- Experiment with additional sentiment analysis models and compare their performance.
- Expand the dataset to include more customer reviews for a more comprehensive analysis.
- Explore advanced techniques for feature engineering and sentiment analysis.
- Visualize the results using interactive charts and graphs.

## Contributing

Contributions to this project are welcome. If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your fork.
5. Submit a pull request with a detailed description of your changes.

## License

This project is licensed under the [MIT License](LICENSE).


