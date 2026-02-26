# Word representations
Hands-on Colab notebooks for tokenization, text representations, and language models
🚧 **Work in Progress** — Notebooks are being added as the courses develop. See the table below for availability.

Course materials exploring how machines turn human language into computable representations — from classical frequency-based methods to modern neural embeddings. Designed for students at the intersection of linguistics and computer science, with no assumption that learners come from only one of those traditions.

Every NLP pipeline begins with the same fundamental question: how do you represent language numerically? The choices made at this stage — how text is split, what counts as a "token," how meaning is encoded — propagate through every downstream task. These notebooks build intuition for those choices by tracing the evolution of representation methods and making their tradeoffs concrete through hands-on exercises.

**Who This Is For**
Students approaching NLP/AI for the first time, who have deep intuitions about language structure but may be new to linear algebra and Python.
CS / programming students who are comfortable with code but may treat language as "just strings" without appreciating the structural and semantic complexity underneath.

**Getting Started**

Clone this repository:
bash   git clone https://github.com/boruizhang/representations.git

Or open any notebook directly in Google Colab using the badges in the table above.
Notebooks are designed to be run sequentially. Each installs its own dependencies via pip in the first cell.

Repo Structure
representations/
├── README.md
├── LICENSE
├── 01_bow-tfidf.ipynb
├── 02_static_embedding.ipynb
├── 03_subword_tokenization.ipynb
├── 06_bert.ipynb
├── 07_gpt.ipynb
├── data/                  # Sample corpora and datasets
    └── README.md          # Data sources and descriptions


**Learning outcomes:**

Start with intuition — Every notebook opens with a linguistic example that exposes why the previous method is insufficient, before introducing the new technique.
Make the math tangible — Equations are always paired with concrete corpus examples. Students compute TF-IDF scores by hand before calling sklearn.
Bridge the two cultures — Exercises alternate between "explain what the code does linguistically" and "implement what this linguistic concept requires computationally."
Trace the historical arc — BOW → TF-IDF → Skip-gram/CBOW → subword tokenization → BERT/GPT follows the actual research trajectory, so students understand not just what each method does but what problem it was invented to solve.
End with the encoder/decoder split — BERT and GPT are taught as two answers to the same question (how to pretrain on unlabeled text), making the architectural differences concrete rather than arbitrary.
