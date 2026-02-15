# Thirsty-lang ML Starter 💧🤖

Machine learning framework examples - data preprocessing, model training, and predictions.

## Features

- Data preprocessing pipelines
- Model training with async operations
- Prediction API
- Model evaluation metrics
- Hyperparameter tuning
- Examples: classification, regression, clustering

## Example: Classification

```thirsty
import { MLModel, DataPreprocessor } from "ml"

glass trainModel() {
  cascade {
    drink data = await loadData("training.csv")
    drink preprocessed = DataPreprocessor.normalize(data)
    
    drink model = MLModel("classification")
    await model.train(preprocessed)
    
    drink accuracy = model.evaluate(testData)
    pour "Accuracy: " + accuracy
  }
}
```

## Included Models

- Linear regression
- Logistic regression  
- Decision trees
- K-means clustering
- Neural networks (basic)

## License

MIT
