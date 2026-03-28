# Multimodal Music Analysis

Ανάλυση και κατηγοριοποίηση μουσικής βάσει δύο διαφορετικών 
modalities: στίχων και ηχητικών χαρακτηριστικών.

## Τι κάνει
- Συλλογή και συνένωση δεδομένων από 5 αρχεία (genres, tags, 
  lyrics, MFCC stats, song info)
- Text Embeddings με BERT (all-MiniLM-L6-v2) από τους στίχους
- Audio Embeddings με Dense Autoencoder (Keras) από MFCC features
- Οπτικοποίηση με t-SNE και Word Clouds ανά genre
- Similarity Analysis με Cosine Similarity για εύρεση όμοιων τραγουδιών

## Αποτελέσματα
Τα audio embeddings διαχωρίζουν καλύτερα τα genres σε σχέση 
με τα text embeddings, με cosine similarity scores 0.97+ για 
ηχητικά παρόμοια τραγούδια.

## Τεχνολογίες
Python · PyTorch · Keras · Sentence-Transformers · 
scikit-learn · pandas · matplotlib · Google Colab
