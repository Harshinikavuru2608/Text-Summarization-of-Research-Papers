# Text-Summarization-of-Research-Papers
Developed a comprehensive text summarizer using abstractive text summarization technique that summarizes text and enables researchers to get precise summary for their work.

In the current era, while doing research in any domain, one of the major task of researchers is to focus on past and present work done in their desired research domain. They have to focus on key points, such as implemented methodology, results, analysis, experimentation, limitations, etc. Use of text summarizer tool will help the researcher in the kick start of their work. We have used Abstractive Text Summarization technique and implemented ”Long Short Term Memory” (LSTM) and PEGASUS model. For training and testing purpose we have used the Ed Collin’s dataset which consists of approximately 10,000 research papers. We provide a detailed comparison of both the techniques. Our results indicate that use of PEGASUS model for long text summarization gives better performance results.

## METHODOLOGY:
A. Data Preprocessing: Figure 1. shows the preprocessing technique used in our implementation.
B. Implementation: Implemented both LSTM and PEGASUS models to see which one works the best for summarization.

## RESULTS:
The LSTM and PEGASUS models are employed to generate abstractive summaries. After fine-tuning the PEGASUS model performed better than LSTM. Fig.2 shows the ROUGE-1, ROUGE-2, and ROUGE-L scores of LSTM model. The precision values of LSTM model are good. This shows us that most of the words produced by the system summary are overlapping with the original summary. However, by observing the output summary produced by LSTM model we observed it has many repeating words, making the summary less sensible.

Fig.3. represents a graph showing ROUGE-1, ROUGE-2, and ROUGE-L scores of PEGASUS model. The model performed much better than LSTM. The ”ROUGE1, ROUGE2, and ROUGE-l” scores of Pegasus improved by 10% compared to the LSTM model. Fig.4 represents the comparison between the F1-scores of both the models. It can be observed that F1-scores of PEGASUS are much higher than LSTM. The recall values in all the ROUGE scores for PEGASUS model are good which indicates that the model’s summary is capturing most parts of the given summary. The output summary shown in Fig.5 is captioned as ”hypothesis”. It can be observed that the ”hypothesis” is very apt to the ”reference” which is the original summary. Thus, we can say that the performance improved greatly compared to LSTM.
