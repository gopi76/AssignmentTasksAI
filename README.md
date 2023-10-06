Certainly! Below is your Python code formatted into a GitHub README with beautiful step-by-step instructions:

---

# Hinglish translation from English text
![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue)


This utility demonstrates the power of transliteration and translation to convert English text into a blend of Hindi and English (Hinglish). It serves as a practical example for:

- Extracting top keywords from a sentence.
- Translating numbers into Hindi numerals.
- Transliterating English words into the Devanagari script.
- Translating transliterated words into Hindi or retaining them as-is (Hinglish).
- Calculating BLEU scores to evaluate translation quality.

## Table of Contents

- [Usage](#usage)
- [Dependencies](#dependencies)
- [How It Works](#how-it-works)
- [Example](#example)

## Usage

1. **Installation**:

   Make sure you have the required Python libraries installed using `pip`:

   ```bash
   pip install indic-transliteration spacy googletrans==4.0.0-rc1 nltk
   ```

2. **Download SpaCy Model**:

   Download the spaCy English language model:

   ```bash
   python -m spacy download en_core_web_sm
   ```

3. **Customize Input Sentences**:

   Replace the sample sentences in the `sentences` list located in the `main()` function with your own input sentences.

4. **Run the Script**:

   Execute the assignment.py code
   ```

5. **Review Results**:

   The script will process each sentence, generate a Hinglish translation, and calculate the BLEU score.

6. **Integration**:

   Integrate these functions into your own projects or applications for text transliteration and translation.

**Note**: Respect usage policies and rate limits of the translation service (Google Translate) when using this utility in real-world applications.

## Dependencies

- [indic-transliteration](https://pypi.org/project/indic-transliteration/): For transliteration to the Devanagari script.
- [spacy](https://spacy.io/): For keyword extraction and English text processing.
- [googletrans](https://pypi.org/project/googletrans/): For translation services.
- [nltk](https://pypi.org/project/nltk/): For BLEU score calculation.

## How It Works

This utility processes text through several steps:

1. Keywords (nouns and adjectives) are extracted from the input sentence.
2. Numbers in the input text are converted to Hindi numerals.
3. English words are transliterated into the Devanagari script.
4. Transliterated words are translated into Hindi or retained as-is (Hinglish) randomly.
5. BLEU scores are calculated to evaluate translation quality.

## Example

Here's an example of how to use this utility:

```python
from transliteration_translation_utility import main

if __name__ == "__main__":
    main()
```
### Example Output

```plaintext
Input Sentence: I had about a 30 minute demo just using this new headset
Hinglish Translation: ई हद् अबोउत् ए ३० minute demo जुस्त् उसिन्ग् थिस् new headset
Bleu Score: 3.9876353728947065e-78

Input Sentence: Definitely share your feedback in the comment section.
Hinglish Translation: डेफ़िनितेल्य् शेयर करना योउर् feedback इन् थे comment बेंडन भी।
Bleu Score: 1.2183324802375697e-231

Input Sentence: So even if it's a big video, I will clearly mention all the products.
Hinglish Translation: दिखाओ एवेन् इफ़् इसका अ big विदेओ, ई विल्ल् च्लेअर्ल्य् मेन्तिओन् अल्ल् थे परियोजनाएं।
Bleu Score: 9.418382295637229e-232
```
