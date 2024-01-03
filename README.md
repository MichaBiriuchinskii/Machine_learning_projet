# Machine_learning_projet
Repository created to collaborate on the studying project in the field of Machine learning. 

Le rapport est [ici](https://docs.google.com/document/d/1nFUwdQ7_tfR2HPpY0eWhLwT_WDBs5a3yFTylqUMHdVQ/edit?usp=sharing)

clean_train_dictionary.pkl.zip

C'est un dico avec les docs lemmatisés et nettoyés qui a la structure : 

{'data_test_en': array([['text', 'label], ..., ['text', 'label]], dtype='<...'),

'data_test_fr': array([['texte', 'label], ..., ['texte', 'label]], dtype='<...'),

'data_test_it': array([['texto', 'labella], ..., ['texto', 'labella]], dtype='<...')}

## Comment traiter pickled dicos ? 

```python
import pickle

# save dictionary to person_data.pkl file
with open('clean_test_dictionary.pkl', 'wb') as fp:
    pickle.dump(dico, fp)
    print('dictionary saved successfully to file')
```


```python
# Read dictionary pkl file
with open('/Users/Michel/Desktop/TAL/MACHINE_LEARNING?/projet/clean_train_dictionary.pkl', 'rb') as fp:
    clean_train_dictionary = pickle.load(fp)

with open('/Users/Michel/Desktop/TAL/MACHINE_LEARNING?/projet/clean_test_dictionary.pkl', 'rb') as fp:
    clean_test_dictionary = pickle.load(fp)

with open('/Users/Michel/Desktop/TAL/MACHINE_LEARNING?/projet/dirty_train_dictionary.pkl', 'rb') as fp:
    dirty_train_dictionary = pickle.load(fp)

with open('/Users/Michel/Desktop/TAL/MACHINE_LEARNING?/projet/dirty_test_dictionary.pkl', 'rb') as fp:
    dirty_test_dictionary = pickle.load(fp)
```
