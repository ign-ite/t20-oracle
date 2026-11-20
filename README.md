# T20 Oracle

Predict the winner of a T20 cricket match with machine learning, trained on 11,000+ historical games.

The models use features such as teams, venue, toss and recent performance. A small FastAPI backend serves predictions (`backend/`), and the training notebooks are in `Notebooks/`.

## What's done

- Trained and compared Logistic Regression, Random Forest and XGBoost
- Hyperparameter tuning with GridSearchCV
- Evaluated with accuracy, log loss and Brier score
- FastAPI service around the trained model

## Results and limitations

Evaluation figures are being re-checked, so they are not published here yet. _(Pending: confirmation of a possible data-leakage issue in the feature pipeline.)_

## What's next

- Save trained models to disk for reuse
- Match simulator: `simulate_match(teamA, teamB)`
- User-defined teams (for example India vs RCB)
- Add a web interface (Streamlit or Flask)
