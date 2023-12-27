# Machine_learning_projet
Repository created to collaborate on the studying project in the field of Machine learning. 


clean_train_dictionary.pkl.zip

C'est un dico avec les docs lemmatisés et nettoyés qui a la structure : 

{'data_test_en': array([['text', 'label], ..., ['text', 'label]], dtype='<...'),

'data_test_fr': array([['texte', 'label], ..., ['texte', 'label]], dtype='<...'),

'data_test_it': array([['texto', 'labella], ..., ['texto', 'labella]], dtype='<...')}

## Comment traiter pickled dicos ? 

```python
rt pickle

# save dictionary to person_data.pkl file
with open('clean_test_dictionary.pkl', 'wb') as fp:
    pickle.dump(dico, fp)
    print('dictionary saved successfully to file')
```


```python
# Read dictionary pkl file
with open('clean_test_dictionary.pkl', 'rb') as fp:
    file = pickle.load(fp)

file.keys()
```
