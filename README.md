**Project Title: TOPSIS for Pretrained Models on Text Conversational
Data**

**Overview**

The TOPSIS (Technique for Order of Preference by Similarity to Ideal
Solution) method is employed to evaluate and rank pretrained models
based on their performance in generating text in conversational
contexts. This evaluation includes considerations such as accuracy,
fluency, coherence, relevance, and training time.

**Models and Evaluation Metrics:**

1.  **GPT-2:**

    -   Model Type: GPT-2 Language Model

    -   Evaluation Metrics: Accuracy, Fluency, Coherence, Relevance

2.  **T5:**

    -   Model Type: T5 Text-to-Text Transformer

    -   Evaluation Metrics: Accuracy, Fluency, Coherence, Relevance

3.  **BERT:**

    -   Model Type: BERT Sequence Classification

    -   Evaluation Metrics: Accuracy, Fluency, Coherence, Relevance

4.  **DistilBERT:**

    -   Model Type: DistilBERT Sequence Classification

    -   Evaluation Metrics: Accuracy, Fluency, Coherence, Relevance

5.  **XLNet:**

    -   Model Type: XLNet Sequence Classification

    -   Evaluation Metrics: Accuracy, Fluency, Coherence, Relevance

**Evaluation Process:**

1.  **Data Preparation:**

    -   Conversational data is loaded from a JSON file, containing a
        list of messages.

2.  **Model Evaluation:**

    -   Each model is evaluated on the basis of accuracy, fluency,
        coherence, and relevance for generating responses in a
        conversational context.

3.  **TOPSIS Calculation:**

    -   The evaluated scores are then normalized and used in the TOPSIS
        algorithm.

    -   Additional consideration is given to training time, with a
        weight assigned for its influence in the overall evaluation.

4.  **Ranking:**

    -   Models are ranked based on their TOPSIS scores, representing an
        aggregate performance measure.

**Results and Output:**

-   The final results provide a comprehensive ranking of pretrained
    models, indicating which models perform better in generating text
    for conversational data.

  -----------------------------------------------------------------------
  **Model**               **Topsis Score**        **Rank**
  ----------------------- ----------------------- -----------------------
  XLNet                   0.0769                  1

  GPT-2                   0.0500                  2

  BERT                    0.0467                  3\|

  DistilBERT              0.0273                  4

  T5                      0.0000                  5
  -----------------------------------------------------------------------

**2. Bar Chart**

![](vertopal_91a028daad1e4b70b5472c089433d7ed/media/image1.png){width="6.268055555555556in"
height="4.35in"}

**File Structure:**

-   **Topsis.py:** Python script containing the TOPSIS evaluation code.

-   **barchart.png**: Bar chart visualizing the model comparison.

-   **text_conv.json:** JSON file containing the conversational data.

-   **README.md:** Overview of the TOPSIS evaluation for pretrained
    models on text conversational data.

-   **Result.csv :** CSV file with ranked results in tabular form

**Usage:**

-   Run **main.py** to execute the evaluation and obtain the ranking of
    pretrained models.

**Dependencies:**

-   Ensure the required Python libraries (e.g., transformers, numpy,
    prettytable) are installed.

**Notes:**

-   Adjust weights or evaluation metrics in the code as needed.

-   GPT-2 outperforms other models securing the top rank. GPT-2 and BERT
    follow closely, showcasing competitive performance. Efficiency
    Consideration: XLnet is the most resource-efficient, with the lowest
    training time. T5 ranks last and doesn't performs well. Next Steps:
    Feel free to analyze the provided CSV files for more insights.
    Consider adjusting the evaluation metrics or adding new models based
    on your specific use case. Use the project as a foundation for
    ongoing research and development in text summarization.
