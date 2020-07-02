About the Dataset:
The dataset contains data of companies having various factors as independent variables or features and profit as dependent variable or the label we have to predict.

Equation: b0+b1x1+b2x2+...+bnxn

Methods of building models:
1) All-in(Using all the data for model if you are sure that all predictors are significant or you are going to perform backward elimination)
2) Backward Elimination(Select a significance level to stay in model->Fit the model with all predictors->Take predictor with highest P-value(if p>SL)->Remove predictor->Fit model->Step3 until highest p<SL).
3) Forward Selection.
4) Bidirectional Elimination(Select SL to enter and SL to stay in model->new variables must have p<SLEnter to entere model->Perform all steps of backward elimination(old variables must have p<SLStay to stay->go to step 2->No new variables can enter and no old can exit->Finish)
5) Score Comparison