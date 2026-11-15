# Assignments

## Part B: Price Whisperer, a game for learning data science concepts

🎮 **Play the game:** https://laxminivasmaroju.github.io/realestate_agent_game/
📄 **Game file:** `index.html`

### About the game
You are the top real estate agent in town. A customer wants a fair price for a house. You build a machine-learning pipeline on real house data, and the model quotes the price. If the quote is close to the true sale price, you close the deal and your reputation grows. If it is far off, the customer walks away and your reputation falls. The game has 5 levels, and the data gets harder each time.

### Learning objectives
After playing, a learner should be able to:
1. Read a data profile (min, max, mean, blanks) to spot problems before modelling.
2. Choose how to handle **missing values** (mean, median, zero, drop) and explain why median is safer.
3. Detect and treat **outliers** using the 1.5 × IQR rule.
4. Encode a **categorical feature** correctly (one-hot vs label encoding).
5. Recognise **data leakage**: a column that is not available when a new house is listed.
6. Explain **overfitting**: with few rows, useless columns let the model memorise noise.
7. Explain why modelling **log(price)** suits prices that grow by percentages.

### How to play
1. Read the **Data profile** table. Look at the blank counts and the largest values.
2. Build your pipeline by choosing features and a setting for each step shown.
3. Press **Run pipeline**. The model trains on 75% of the houses and is tested on 25% it has never seen.
4. If you win, you move to the next level. If you lose, read the explanation, adjust and retry. Each failed attempt costs reputation.
5. At the end, the **coach report** shows each mistake, the data evidence behind it, what to do instead, and how much error that fix would remove.

### Levels
| Level | Name | Concept taught |
|---|---|---|
| 1 | Clean Start | Feature choice, regression, log target |
| 2 | Messy Listings | Missing values and outliers |
| 3 | The Trap | Categorical encoding and data leakage |
| 4 | Small Town | Overfitting from too many useless columns |
| 5 | Market Boss | All of the above combined |

### How it works
- Everything runs in the browser. There is no backend and no hard-coded answers.
- Each level generates a house dataset with a fixed random seed.
- The pipeline performs real computation: imputation, outlier removal, encoding and a linear regression fitted by the normal equations.
- Your result is the average percentage error on unseen houses. It is compared with an expert pipeline for that level.
- When you lose, the game re-runs your pipeline with one step at a time swapped for the expert choice. This shows exactly which step cost you the most.

### Playtest evidence
| Playtester | Level reached | Final reputation | Feedback |
|---|---|---|---|
| (name) | | | |
| (name) | | | |
| (name) | | | |

**What I changed after playtesting:**
- (write one or two changes you made, or planned, based on feedback)

---

## Other assignment: Nifty50 pipeline
Files: `nifty50_pipeline.ipynb` and `ADANI_ENTERPRISES.CSV`
