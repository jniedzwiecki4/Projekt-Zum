# Projekt-Zum

## Dane

W badaniu wykorzystałem dataset [Toxic Tweets Dataset](https://www.kaggle.com/datasets/ashwiniyer176/toxic-tweets-dataset). Jest to zbiór danych składajacy się z wpisów z platformy twitter oraz kolumny określającej czy dany tweet jest toksyczny czy nie. Dataset zawiera podobną ilość danych dla obu klas. 

## Instrukcja

Badanie zostało przeprowadzone w pliku projektZUM.ipynb. Pierwszy chunk notebooka określa jakie paczki należy uprzednio zainstalować. FinalBalancedDataset.csv zawiera dane wykorzystane w badaniu.

## Opisy modelów

### Model LSTM

Składa się z warstwy Embedding, dwukierunkowej warstwy LSTM oraz dwóch warstw Dense. Pierwsza z warstw dense ma funkcję aktywacji relu a ostatnia sigmoid. Skorzystano z optymalizatora Adama.

### Model CNN

Składa się z warstwy Embedding, Conv1D, GlobalMaxPooling1D oraz dwóch warst Dense. Pierwsza z warstw dense ma funkcję aktywacji relu a ostatnia sigmoid. Skorzystano z optymalizatora Adama.

### Fine tuning modelu z pre-trained word-embeddingiem oraz fine tuning modelu językowego

W pozostałych dwóch modelach został wykorzystany distilbert-base-uncased. Skorzystano z optymalizatora Adama.
