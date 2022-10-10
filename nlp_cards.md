# Natural Language Processsing Cards
NLP is a broad field,

## Preprocessing
- lemmatization
- stop words
- tokenization

## Models
### Transformers
- Bert - bi-directional transformer
  - Sentiment analysis
  - Named Entity Recognition (NER)
  - Question Answering (QA)
  - Text Prediction - next word
  - Text Generation
  - Summarization
  - Polysemy resolution 
    - differentiate words with multiple meanings, e.g. "bank", based on context



### Embeddings
- Continuous Bag-of-words
- GLoVe
- word2vec

## Tasks

### Transcription 
Aka, Speech to Text or Automatic Speech Recognition (ASR). Includes diarization, meaning who's talking.
- OpenAI's [Whisper](https://openai.com/blog/whisper/), opensource, bi-directional
  - includes punctuation, didn't see diarization
  - tiny, base, small, medium, large
    - small-large do a good job recognizing non-english/marketing words
  - [training data](https://github.com/openai/whisper/blob/main/model-card.md#training-data)
    - 680k hours of multi-lingual and multi-task supervised data from the web, 65% english
    - 30 second snippets
  - speech-to-text translation
  - "predictions may include texts that are not actually spoken in the audio input (i.e. hallucination)"
  - Q's: custom vocab, fine-tuning
- [AWS Transcribe](https://aws.amazon.com/transcribe/), closed source, paid
  - batch and streaming, sub-flavor Transcribe Medical (expensive) will id PHI
  - language identification, diarization, punctuation, number formatting
  - custom vocabulary for domain specific language
  - Custom Language Model based on a corpus of text data

<!-- TODO: text EDA, Language Recognition,  NER, Sentiment Analysis, Question Answering, Summarization -->


## Packages
- SpaCy
- Stanford's NLTK
