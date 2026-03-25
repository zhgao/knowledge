BM25
	Type: Lexical (keyword-based) retrieval
	Used in: Traditional search engines (Elasticsearch, Lucene)

	How it works

		BM25 ranks documents based on:

			Term frequency (how often a word appears)
			Inverse document frequency (how rare the word is)
			Document length normalization

		👉 It matches exact words between query and documents.

		Key characteristics
			No embeddings
			No semantic understanding
			Fast and lightweight
			Works best for exact keyword matching
	Example

		Query: "bank transfer delay"

		BM25 will favor documents containing:

		“bank”
		“transfer”
		“delay”

	Even if the meaning is similar but words differ, it may miss them.
