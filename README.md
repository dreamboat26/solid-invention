# Recurring Spans: Self-Supervised Anchor, Positive, and Negative Construction

This notebook presents the concept of Recurring Spans, a strategy used for self-supervised anchor, positive, and negative construction in the paper "Learning to Retrieve Passages without Supervision" by Ram et al. (2022).

The process involves four main steps:

1. **Chunking Documents into Passages**: The document is divided into 100-word chunks called passages.
2. **Extracting Spans / n-grams**: Spans or n-grams are extracted from each passage.
3. **Counting Recurring Spans**: The recurring spans across passages are counted.
4. **Sorting Recurring Spans**: Recurring spans are sorted by length, and the longest matching passages are taken as positives.

## Steps in Detail

### 1. Chunking Documents into Passages

The document is divided into smaller, manageable units called passages, each containing 100 words.

### 2. Extracting Spans / n-grams

Spans or n-grams are extracted from each passage. These can be contiguous sequences of words or phrases.

### 3. Counting Recurring Spans

The recurring spans across passages are identified and counted. This helps identify common patterns or phrases that appear multiple times in the document.

### 4. Sorting Recurring Spans

The recurring spans are sorted by length, and the longest matching passages are selected as positives. These passages are likely to contain important information or key phrases related to the document's topic.

## Implementation

The implementation involves Python code to perform the above steps. Each step is explained and demonstrated using code snippets.

# Example Usage:
- document = "This is a sample document. It contains multiple sentences and words. We will divide it into passages and extract spans."
- passages = chunk_document(document)
- spans = extract_spans(passages)
- span_counts = count_recurring_spans(spans)
- recurring_spans = sort_recurring_spans(span_counts)

