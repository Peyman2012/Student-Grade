# Student-Grade

By using this code, the data can be scaled:

    X_train=df['Hours'].values.reshape(-1,1)
    y_train=df['Scores'].values.reshape(-1,1)
    X_test=df2['Hours'].values.reshape(-1,1)

It turns the scores above 100 into the maximum scores so that we don't have a score above 100 to have a more beautiful plot

   y_pred_test = np.clip(y_pred2, 0, 100)
