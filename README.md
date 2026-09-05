# pytorch_proj

PyTorch training/test project: a small binary classifier for the Kaggle
[Titanic](https://www.kaggle.com/competitions/titanic) competition.

## What's here

`pytorch_titanic/` contains the notebooks:

- **pytorch.ipynb** — end-to-end walkthrough: downloads the Titanic dataset via
  the Kaggle API, engineers features (deck, family size, ticket frequency,
  title, etc.), preprocesses with a scikit-learn `ColumnTransformer`, and
  trains a small feed-forward network (`TitanicNet`) in PyTorch to predict
  survival.
- **pytorch_model2.ipynb** — a second iteration of the model.

## Setup

1. Create and activate a virtual environment, then install dependencies used
   by the notebooks (pandas, numpy, scikit-learn, torch, kaggle, python-dotenv,
   matplotlib).
2. Add your Kaggle API token to a local `.env` file:

   ```
   KAGGLE_API_TOKEN=your_token_here
   ```

3. Run the notebooks in `pytorch_titanic/`. The Titanic dataset is downloaded
   automatically on first run if it isn't already present.
