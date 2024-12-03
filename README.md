# VILLANOS Gendered Corpus

The **VILLANOS Gendered Corpus** is a carefully curated dataset designed to analyze gendered language and the dynamics of textual references to violence and gender. The corpus is annotated with the following categories for each text entry:

- **TEXTO**: The primary text content.
- **VIOLENCIA**: A marker indicating whether the text contains a reference to violence (binary value).
- **Mención MUJER**: An indicator of whether the text mentions women (binary value).
- **Mención HOMBRE**: An indicator of whether the text mentions men (binary value).
- **Dirigido MUJER**: A marker specifying if the text is directed toward women (binary value).
    - For **non-violent messages**, annotators evaluated whether the message was directly addressed to a specific woman or represented a general statement without a clear addressee.
    - For **violent messages**, annotators recorded if a woman was the target of the violence.
- **Dirigido HOMBRE**: A marker specifying if the text is directed toward men (binary value).
    - For **non-violent messages**, annotators evaluated whether the message was directly addressed to a specific man or represented a general statement without a clear addressee.
    - For **violent messages**, annotators recorded if a man was the target of the violence.

### Dataset Files
The base dataset and its derived subsets are as follows:

1. **`data/villanos_manual_gender.csv`**
   - This is the base dataset, manually annotated to serve as the foundational corpus. All other files are derived from this dataset.

2. **`data/villanos_balanced_by_mentions.csv`**
   - A subset of the base dataset where the mentions of women and men are evenly distributed. This ensures a balanced frequency of gender mentions to mitigate bias in analysis.

3. **`data/villanos_balanced_by_targets.csv`**
   - A subset of the base dataset balanced based on the "directed towards" annotations. This guarantees an equal representation of texts directed at women and men.

4. **`data/villanos_debiased_by_mentions.csv`**
   - A subset derived from the base dataset that has undergone debiasing techniques to minimize gender bias related to mentions of women and men.

5. **`data/villanos_debiased_by_targets.csv`**
   - A subset of the base dataset, debiased with respect to the "directed towards" markers, aiming to reduce directional biases in communication.

### Summary

The manually annotated corpus consists of **1000** entries and is designed to support a wide range of computational linguistics and gender studies research. Researchers can explore patterns of gendered language in relation to violence, mentions, and directionality in communication.

### Binary Value Annotations
For the binary values in the dataset:
- `1` indicates **yes/true**.
- `0` indicates **no/false**.

### Access
The data is located in the **`data/`** directory.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />
<span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">VILLANOS Gendered Corpus</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.