# Evaluation questions

## Q1
Type: exact fact
Question: Who makes spaCy, is it a company?
Answer: spaCy is not a company. It is an open-source library, published by a company called Explosion.
Source file: spacy-101.mdx

## Q2
Type: exact fact
Question: What do I get back when I load a spaCy pipeline, and what do people usually call it?
Answer: spacy.load returns a Language object holding all components and data needed to process text. It is usually called nlp.
Source file: spacy-101.mdx

## Q3
Type: how-to
Question: How do I get a small English model onto my computer?
Answer: Run python -m spacy download en_core_web_sm.
Source file: spacy-101.mdx

## Q4
Type: how-to
Question: How do I turn a piece of text into something spaCy can analyse?
Answer: Load a pipeline with spacy.load, for example nlp = spacy.load("en_core_web_sm"), then call nlp on the string. It returns a processed Doc.
Source file: spacy-101.mdx

## Q5
Type: vague or casual
Question: If spaCy chops my sentence into words, do I lose my original spacing?
Answer: No. The Doc keeps all information of the original text, including whitespace, and you can rebuild the original by joining the tokens and their trailing whitespace.
Source file: spacy-101.mdx