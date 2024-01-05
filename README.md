# Language-Processing-
Natural Language Processing with spaCy:
import spacy

# Load spaCy model
nlp = spacy.load("en_core_web_sm")

# Process text
text = "Natural Language Processing is amazing!"
doc = nlp(text)

# Analyze text
for token in doc:
    print(token.text, token.lemma_, token.pos_, token.is_stop)
