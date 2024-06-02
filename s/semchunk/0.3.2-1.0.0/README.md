# Comparing `tmp/semchunk-0.3.2.tar.gz` & `tmp/semchunk-1.0.0.tar.gz`

## Comparing `semchunk-0.3.2.tar` & `semchunk-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 semchunk-0.3.2/CHANGELOG.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 semchunk-0.3.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 semchunk-0.3.2/htmlcov/.gitignore
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 semchunk-0.3.2/src/semchunk/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semchunk-0.3.2/src/semchunk/py.typed
--rw-r--r--   0        0        0    14510 2020-02-02 00:00:00.000000 semchunk-0.3.2/src/semchunk/semchunk.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 semchunk-0.3.2/tests/bench.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 semchunk-0.3.2/tests/test_semchunk.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 semchunk-0.3.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 semchunk-0.3.2/LICENCE
--rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 semchunk-0.3.2/README.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 semchunk-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 semchunk-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 semchunk-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 semchunk-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 semchunk-1.0.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 semchunk-1.0.0/src/semchunk/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semchunk-1.0.0/src/semchunk/py.typed
+-rw-r--r--   0        0        0    14845 2020-02-02 00:00:00.000000 semchunk-1.0.0/src/semchunk/semchunk.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 semchunk-1.0.0/tests/bench.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 semchunk-1.0.0/tests/test_semchunk.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 semchunk-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 semchunk-1.0.0/LICENCE
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 semchunk-1.0.0/README.md
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 semchunk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 semchunk-1.0.0/PKG-INFO
```

### Comparing `semchunk-0.3.2/CHANGELOG.md` & `semchunk-1.0.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 ## Changelog 🔄
 All notable changes to `semchunk` will be documented here. This project adheres to [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.0] - 2024-06-02
+### Added
+- Added a `progress` argument to the chunker returned by `chunkerify()` that, when set to `True` and multiple texts are passed, displays a progress bar.
+
 ## [0.3.2] - 2024-06-01
 ### Fixed
 - Fixed a bug where a `DivisionByZeroError` would be raised where a token counter returned zero tokens when called from `merge_splits()`, courtesy of [@jcobol](https://github.com/jcobol) ([#5](https://github.com/umarbutler/semchunk/pull/5)) ([7fd64eb](https://github.com/umarbutler/semchunk/pull/5/commits/7fd64eb8cf51f45702c59f43795be9a00c7d0d17)), fixing [#4](https://github.com/umarbutler/semchunk/issues/4).
 
 ## [0.3.1] - 2024-05-18
 ### Fixed
 - Fixed typo in error messages in `chunkerify()` where it was referred to as `make_chunker()`.
@@ -52,14 +56,15 @@
 - Improved chunking performance.
 - improved test coverage.
 
 ## [0.1.0] - 2023-11-05
 ### Added
 - Added the `chunk()` function, which splits text into semantically meaningful chunks of a specified size as determined by a provided token counter.
 
+[1.0.0]: https://github.com/umarbutler/semchunk/compare/v0.3.2...v1.0.0
 [0.3.2]: https://github.com/umarbutler/semchunk/compare/v0.3.1...v0.3.2
 [0.3.1]: https://github.com/umarbutler/semchunk/compare/v0.3.0...v0.3.1
 [0.3.0]: https://github.com/umarbutler/semchunk/compare/v0.2.4...v0.3.0
 [0.2.4]: https://github.com/umarbutler/semchunk/compare/v0.2.3...v0.2.4
 [0.2.3]: https://github.com/umarbutler/semchunk/compare/v0.2.2...v0.2.3
 [0.2.2]: https://github.com/umarbutler/semchunk/compare/v0.2.1...v0.2.2
 [0.2.1]: https://github.com/umarbutler/semchunk/compare/v0.2.0...v0.2.1
```

### Comparing `semchunk-0.3.2/.github/workflows/ci.yml` & `semchunk-1.0.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `semchunk-0.3.2/src/semchunk/semchunk.py` & `semchunk-1.0.0/src/semchunk/semchunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from bisect import bisect_left
 from typing import Callable, Sequence, TYPE_CHECKING
 from functools import cache, wraps
 from itertools import accumulate
 from contextlib import suppress
 
+from tqdm import tqdm
+
 if TYPE_CHECKING:
     import tiktoken
     import tokenizers
     import transformers
 
 _memoized_token_counters = {}
 """A map of token counters to their memoized versions."""
@@ -238,22 +240,27 @@
         token_counter = faster_token_counter
     
     # Memoize the token counter if necessary.
     if memoize:
         token_counter = _memoized_token_counters.setdefault(token_counter, cache(token_counter))
     
     # Construct and return the chunker.
-    def chunker(text_or_texts: str | Sequence[str]) -> list[str] | list[list[str]]:
+    def chunker(text_or_texts: str | Sequence[str], progress: bool = False) -> list[str] | list[list[str]]:
         """Split text or texts into semantically meaningful chunks of a specified size as determined by the provided tokenizer or token counter.
         
         Args:
             text_or_texts (str | Sequence[str]): The text or texts to be chunked.
         
         Returns:
-            list[str] | list[list[str]]: If a single text has been provided, a list of chunks up to `chunk_size`-tokens-long, with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts."""
+            list[str] | list[list[str]]: If a single text has been provided, a list of chunks up to `chunk_size`-tokens-long, with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts.
+            progress (bool, optional): Whether to display a progress bar when chunking multiple texts. Defaults to `False`."""
                 
         if isinstance(text_or_texts, str):
             return chunk(text_or_texts, chunk_size, token_counter, memoize = False)
         
-        return [chunk(text, chunk_size, token_counter, memoize = False) for text in text_or_texts]
+        if progress:
+            return [chunk(text, chunk_size, token_counter, memoize = False) for text in tqdm(text_or_texts)]
+        
+        else:
+            return [chunk(text, chunk_size, token_counter, memoize = False) for text in text_or_texts]
     
     return chunker
```

### Comparing `semchunk-0.3.2/tests/bench.py` & `semchunk-1.0.0/tests/bench.py`

 * *Files identical despite different names*

### Comparing `semchunk-0.3.2/tests/test_semchunk.py` & `semchunk-1.0.0/tests/test_semchunk.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,8 +78,11 @@
     try:
         chunker = semchunk.chunkerify('\n\f\rع\n\f\r', 1)
         worked = False
     
     except ValueError:
         worked = True
     
-    assert worked
+    assert worked
+    
+    # Try enabling a progress bar.
+    chunker(['ThisIs\tATest.', 'ThisIs\tATest.'], progress = True)
```

### Comparing `semchunk-0.3.2/LICENCE` & `semchunk-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `semchunk-0.3.2/README.md` & `semchunk-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # semchunk
-<a href="https://pypi.org/project/semchunk/" alt="PyPI Version"><img src="https://img.shields.io/pypi/v/semchunk"></a> <a href="https://github.com/umarbutler/semchunk/actions/workflows/ci.yml" alt="Build Status"><img src="https://img.shields.io/github/actions/workflow/status/umarbutler/semchunk/ci.yml?branch=main"></a> <a href="https://app.codecov.io/gh/umarbutler/semchunk" alt="Code Coverage"><img src="https://img.shields.io/codecov/c/github/umarbutler/semchunk"></a> <!-- <a href="https://pypistats.org/packages/semchunk" alt="Downloads"><img src="https://img.shields.io/pypi/dm/semchunk"></a> -->
+<a href="https://pypi.org/project/semchunk/" alt="PyPI Version"><img src="https://img.shields.io/pypi/v/semchunk"></a> <a href="https://github.com/umarbutler/semchunk/actions/workflows/ci.yml" alt="Build Status"><img src="https://img.shields.io/github/actions/workflow/status/umarbutler/semchunk/ci.yml?branch=main"></a> <a href="https://app.codecov.io/gh/umarbutler/semchunk" alt="Code Coverage"><img src="https://img.shields.io/codecov/c/github/umarbutler/semchunk"></a> <a href="https://pypistats.org/packages/semchunk" alt="Downloads"><img src="https://img.shields.io/pypi/dm/semchunk"></a>
 
 `semchunk` is a fast and lightweight pure Python library for splitting text into semantically meaningful chunks.
 
 Owing to its complex yet highly efficient chunking algorithm, `semchunk` is both more semantically accurate than [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://python.langchain.com/docs/modules/data_connection/document_transformers/text_splitters/recursive_text_splitter) (see [How It Works 🔍](https://github.com/umarbutler/semchunk#how-it-works-)) and is also over 90% faster than [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) (see the [Benchmarks 📊](https://github.com/umarbutler/semchunk#benchmarks-)).
 
 ## Installation 📦
 `semchunk` may be installed with `pip`:
@@ -31,15 +31,15 @@
           semchunk.chunkerify(AutoTokenizer.from_pretrained('umarbutler/emubert'), chunk_size) or \
           semchunk.chunkerify(tiktoken.encoding_for_model('gpt-4'), chunk_size) or \
           semchunk.chunkerify(lambda text: len(text.split()), chunk_size)
 
 # The resulting `chunker` can take and chunk a single text or a list of texts, returning a list of
 # chunks or a list of lists of chunks, respectively.
 assert chunker(text) == ['The quick', 'brown', 'fox', 'jumps', 'over the', 'lazy', 'dog.']
-assert chunker([text]) == [['The quick', 'brown', 'fox', 'jumps', 'over the', 'lazy', 'dog.']]
+assert chunker([text], progress = True) == [['The quick', 'brown', 'fox', 'jumps', 'over the', 'lazy', 'dog.']]
 ```
 
 ### Chunkerify
 ```python
 def chunkerify(
     tokenizer_or_token_counter: str | tiktoken.Encoding | transformers.PreTrainedTokenizer | \
                                 tokenizers.Tokenizer | Callable[[str], int],
@@ -55,15 +55,15 @@
 
 `chunk_size` is the maximum number of tokens a chunk may contain. It defaults to `None` in which case it will be set to the same value as the tokenizer's `model_max_length` attribute (deducted by the number of tokens returned by attempting to tokenize an empty string) if possible otherwise a `ValueError` will be raised.
 
 `max_token_chars` is the maximum numbers of characters a token may contain. It is used to significantly speed up the token counting of long inputs. It defaults to `None` in which case it will either not be used or will, if possible, be set to the numbers of characters in the longest token in the tokenizer's vocabulary as determined by the `token_byte_values` or `get_vocab` methods.
 
 `memoize` flags whether to memoize the token counter. It defaults to `True`.
 
-This function returns a callable that takes either a single text or a sequence of texts and returns, if a single text has been provided, a list of chunks up to `chunk_size`-tokens-long with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts.
+This function returns a callable that takes either a single text or a sequence of texts and returns, if a single text has been provided, a list of chunks up to `chunk_size`-tokens-long with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts. The callable can also be passed a `progress` argument which if set to `True` and multiple texts are passed, will display a progress bar.
 
 ### Chunk
 ```python
 def chunk(
     text: str,
     chunk_size: int,
     token_counter: Callable,
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # semchunk _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_s_e_m_c_h_u_n_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_/_c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_c_o_v_/_c_/_g_i_t_h_u_b_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_]`semchunk` is a fast and
-lightweight pure Python library for splitting text into semantically meaningful
-chunks. Owing to its complex yet highly efficient chunking algorithm,
-`semchunk` is both more semantically accurate than
-[`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://
-python.langchain.com/docs/modules/data_connection/document_transformers/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_c_o_v_/_c_/_g_i_t_h_u_b_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_p_y_p_i_/_d_m_/_s_e_m_c_h_u_n_k_]`semchunk` is a fast and lightweight pure Python library for
+splitting text into semantically meaningful chunks. Owing to its complex yet
+highly efficient chunking algorithm, `semchunk` is both more semantically
+accurate than [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https:
+//python.langchain.com/docs/modules/data_connection/document_transformers/
 text_splitters/recursive_text_splitter) (see [How It Works ð](https://
 github.com/umarbutler/semchunk#how-it-works-)) and is also over 90% faster than
 [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/)
 (see the [Benchmarks ð](https://github.com/umarbutler/semchunk#benchmarks-
 )). ## Installation ð¦ `semchunk` may be installed with `pip`: ```bash pip
 install semchunk ``` ## Usage ð©âð» The code snippet below demonstrates
 how text can be chunked with `semchunk`: ```python import semchunk from
@@ -26,25 +26,25 @@
 ('gpt-4', chunk_size) or \ semchunk.chunkerify('cl100k_base', chunk_size) or \
 semchunk.chunkerify(AutoTokenizer.from_pretrained('umarbutler/emubert'),
 chunk_size) or \ semchunk.chunkerify(tiktoken.encoding_for_model('gpt-4'),
 chunk_size) or \ semchunk.chunkerify(lambda text: len(text.split()),
 chunk_size) # The resulting `chunker` can take and chunk a single text or a
 list of texts, returning a list of # chunks or a list of lists of chunks,
 respectively. assert chunker(text) == ['The quick', 'brown', 'fox', 'jumps',
-'over the', 'lazy', 'dog.'] assert chunker([text]) == [['The quick', 'brown',
-'fox', 'jumps', 'over the', 'lazy', 'dog.']] ``` ### Chunkerify ```python def
-chunkerify( tokenizer_or_token_counter: str | tiktoken.Encoding |
-transformers.PreTrainedTokenizer | \ tokenizers.Tokenizer | Callable[[str],
-int], chunk_size: int = None, max_token_chars: int = None, memoize: bool =
-True, ) -> Callable[[str | Sequence[str]], list[str] | list[list[str]]]: ```
-`chunkerify()` constructs a chunker that splits one or more texts into
-semantically meaningful chunks of a specified size as determined by the
-provided tokenizer or token counter. `tokenizer_or_token_counter` is either:
-the name of a `tiktoken` or `transformers` tokenizer (with priority given to
-the former); a tokenizer that possesses an `encode` attribute (eg, a
+'over the', 'lazy', 'dog.'] assert chunker([text], progress = True) == [['The
+quick', 'brown', 'fox', 'jumps', 'over the', 'lazy', 'dog.']] ``` ###
+Chunkerify ```python def chunkerify( tokenizer_or_token_counter: str |
+tiktoken.Encoding | transformers.PreTrainedTokenizer | \ tokenizers.Tokenizer |
+Callable[[str], int], chunk_size: int = None, max_token_chars: int = None,
+memoize: bool = True, ) -> Callable[[str | Sequence[str]], list[str] | list
+[list[str]]]: ``` `chunkerify()` constructs a chunker that splits one or more
+texts into semantically meaningful chunks of a specified size as determined by
+the provided tokenizer or token counter. `tokenizer_or_token_counter` is
+either: the name of a `tiktoken` or `transformers` tokenizer (with priority
+given to the former); a tokenizer that possesses an `encode` attribute (eg, a
 `tiktoken`, `transformers` or `tokenizers` tokenizer); or a token counter that
 returns the number of tokens in a input. `chunk_size` is the maximum number of
 tokens a chunk may contain. It defaults to `None` in which case it will be set
 to the same value as the tokenizer's `model_max_length` attribute (deducted by
 the number of tokens returned by attempting to tokenize an empty string) if
 possible otherwise a `ValueError` will be raised. `max_token_chars` is the
 maximum numbers of characters a token may contain. It is used to significantly
@@ -53,46 +53,48 @@
 characters in the longest token in the tokenizer's vocabulary as determined by
 the `token_byte_values` or `get_vocab` methods. `memoize` flags whether to
 memoize the token counter. It defaults to `True`. This function returns a
 callable that takes either a single text or a sequence of texts and returns, if
 a single text has been provided, a list of chunks up to `chunk_size`-tokens-
 long with any whitespace used to split the text removed, or, if multiple texts
 have been provided, a list of lists of chunks, with each inner list
-corresponding to the chunks of one of the provided input texts. ### Chunk
-```python def chunk( text: str, chunk_size: int, token_counter: Callable,
-memoize: bool = True, ) -> list[str] ``` `chunk()` splits a text into
-semantically meaningful chunks of a specified size as determined by the
-provided token counter. `text` is the text to be chunked. `chunk_size` is the
-maximum number of tokens a chunk may contain. `token_counter` is a callable
-that takes a string and returns the number of tokens in it. `memoize` flags
-whether to memoize the token counter. It defaults to `True`. This function
-returns a list of chunks up to `chunk_size`-tokens-long, with any whitespace
-used to split the text removed. ## How It Works ð `semchunk` works by
-recursively splitting texts until all resulting chunks are equal to or less
-than a specified chunk size. In particular, it: 1. Splits text using the most
-semantically meaningful splitter possible; 1. Recursively splits the resulting
-chunks until a set of chunks equal to or less than the specified chunk size is
-produced; 1. Merges any chunks that are under the chunk size back together
-until the chunk size is reached; and 1. Reattaches any non-whitespace splitters
-back to the ends of chunks barring the final chunk if doing so does not bring
-chunks over the chunk size, otherwise adds non-whitespace splitters as their
-own chunks. To ensure that chunks are as semantically meaningful as possible,
-`semchunk` uses the following splitters, in order of precedence: 1. The largest
-sequence of newlines (`\n`) and/or carriage returns (`\r`); 1. The largest
-sequence of tabs; 1. The largest sequence of whitespace characters (as defined
-by regex's `\s` character class); 1. Sentence terminators (`.`, `?`, `!` and
-`*`); 1. Clause separators (`;`, `,`, `(`, `)`, `[`, `]`, `â`, `â`, `â`,
-`â`, `'`, `"` and `` ` ``); 1. Sentence interrupters (`:`, `â` and `â¦`);
-1. Word joiners (`/`, `\`, `â`, `&` and `-`); and 1. All other characters.
-`semchunk` also relies on memoization to cache the results of token counters
-and the `chunk()` function, thereby improving performance. ## Benchmarks ð
-On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it
-takes `semchunk` 8.34 seconds to split every sample in [NLTK's Gutenberg
-Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-
-token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18
-texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`]
-(https://pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the
-same texts into 512-token-long chunks â a difference of 92.84%. The code used
-to benchmark `semchunk` and `semantic-text-splitter` is available [here](https:
-//github.com/umarbutler/semchunk/blob/main/tests/bench.py). ## Licence ð
-This library is licensed under the [MIT License](https://github.com/umarbutler/
+corresponding to the chunks of one of the provided input texts. The callable
+can also be passed a `progress` argument which if set to `True` and multiple
+texts are passed, will display a progress bar. ### Chunk ```python def chunk
+( text: str, chunk_size: int, token_counter: Callable, memoize: bool = True, )
+-> list[str] ``` `chunk()` splits a text into semantically meaningful chunks of
+a specified size as determined by the provided token counter. `text` is the
+text to be chunked. `chunk_size` is the maximum number of tokens a chunk may
+contain. `token_counter` is a callable that takes a string and returns the
+number of tokens in it. `memoize` flags whether to memoize the token counter.
+It defaults to `True`. This function returns a list of chunks up to
+`chunk_size`-tokens-long, with any whitespace used to split the text removed.
+## How It Works ð `semchunk` works by recursively splitting texts until all
+resulting chunks are equal to or less than a specified chunk size. In
+particular, it: 1. Splits text using the most semantically meaningful splitter
+possible; 1. Recursively splits the resulting chunks until a set of chunks
+equal to or less than the specified chunk size is produced; 1. Merges any
+chunks that are under the chunk size back together until the chunk size is
+reached; and 1. Reattaches any non-whitespace splitters back to the ends of
+chunks barring the final chunk if doing so does not bring chunks over the chunk
+size, otherwise adds non-whitespace splitters as their own chunks. To ensure
+that chunks are as semantically meaningful as possible, `semchunk` uses the
+following splitters, in order of precedence: 1. The largest sequence of
+newlines (`\n`) and/or carriage returns (`\r`); 1. The largest sequence of
+tabs; 1. The largest sequence of whitespace characters (as defined by regex's
+`\s` character class); 1. Sentence terminators (`.`, `?`, `!` and `*`); 1.
+Clause separators (`;`, `,`, `(`, `)`, `[`, `]`, `â`, `â`, `â`, `â`,
+`'`, `"` and `` ` ``); 1. Sentence interrupters (`:`, `â` and `â¦`); 1. Word
+joiners (`/`, `\`, `â`, `&` and `-`); and 1. All other characters. `semchunk`
+also relies on memoization to cache the results of token counters and the
+`chunk()` function, thereby improving performance. ## Benchmarks ð On a
+desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it takes
+`semchunk` 8.34 seconds to split every sample in [NLTK's Gutenberg Corpus]
+(https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long
+chunks with GPT-4's tokenizer (for context, the Corpus contains 18 texts and
+3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://
+pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the same
+texts into 512-token-long chunks â a difference of 92.84%. The code used to
+benchmark `semchunk` and `semantic-text-splitter` is available [here](https://
+github.com/umarbutler/semchunk/blob/main/tests/bench.py). ## Licence ð This
+library is licensed under the [MIT License](https://github.com/umarbutler/
 semchunk/blob/main/LICENCE).
```

### Comparing `semchunk-0.3.2/pyproject.toml` & `semchunk-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "semchunk"
-version = "0.3.2"
+version = "1.0.0"
 authors = [
   {name="Umar Butler", email="umar@umar.au"},
 ]
 description = "A fast and lightweight pure Python library for splitting text into semantically meaningful chunks."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="MIT"}
@@ -41,14 +41,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: General",
     "Topic :: Utilities",
     "Typing :: Typed"
 ]
 dependencies = [
+    "tqdm",
 ]
 
 [project.urls]
 Homepage = "https://github.com/umarbutler/semchunk"
 Documentation = "https://github.com/umarbutler/semchunk/blob/main/README.md"
 Issues = "https://github.com/umarbutler/semchunk/issues"
 Source = "https://github.com/umarbutler/semchunk"
```

### Comparing `semchunk-0.3.2/PKG-INFO` & `semchunk-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: semchunk
-Version: 0.3.2
+Version: 1.0.0
 Summary: A fast and lightweight pure Python library for splitting text into semantically meaningful chunks.
 Project-URL: Homepage, https://github.com/umarbutler/semchunk
 Project-URL: Documentation, https://github.com/umarbutler/semchunk/blob/main/README.md
 Project-URL: Issues, https://github.com/umarbutler/semchunk/issues
 Project-URL: Source, https://github.com/umarbutler/semchunk
 Author-email: Umar Butler <umar@umar.au>
 License: MIT
@@ -25,18 +25,19 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # semchunk
-<a href="https://pypi.org/project/semchunk/" alt="PyPI Version"><img src="https://img.shields.io/pypi/v/semchunk"></a> <a href="https://github.com/umarbutler/semchunk/actions/workflows/ci.yml" alt="Build Status"><img src="https://img.shields.io/github/actions/workflow/status/umarbutler/semchunk/ci.yml?branch=main"></a> <a href="https://app.codecov.io/gh/umarbutler/semchunk" alt="Code Coverage"><img src="https://img.shields.io/codecov/c/github/umarbutler/semchunk"></a> <!-- <a href="https://pypistats.org/packages/semchunk" alt="Downloads"><img src="https://img.shields.io/pypi/dm/semchunk"></a> -->
+<a href="https://pypi.org/project/semchunk/" alt="PyPI Version"><img src="https://img.shields.io/pypi/v/semchunk"></a> <a href="https://github.com/umarbutler/semchunk/actions/workflows/ci.yml" alt="Build Status"><img src="https://img.shields.io/github/actions/workflow/status/umarbutler/semchunk/ci.yml?branch=main"></a> <a href="https://app.codecov.io/gh/umarbutler/semchunk" alt="Code Coverage"><img src="https://img.shields.io/codecov/c/github/umarbutler/semchunk"></a> <a href="https://pypistats.org/packages/semchunk" alt="Downloads"><img src="https://img.shields.io/pypi/dm/semchunk"></a>
 
 `semchunk` is a fast and lightweight pure Python library for splitting text into semantically meaningful chunks.
 
 Owing to its complex yet highly efficient chunking algorithm, `semchunk` is both more semantically accurate than [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://python.langchain.com/docs/modules/data_connection/document_transformers/text_splitters/recursive_text_splitter) (see [How It Works 🔍](https://github.com/umarbutler/semchunk#how-it-works-)) and is also over 90% faster than [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) (see the [Benchmarks 📊](https://github.com/umarbutler/semchunk#benchmarks-)).
 
 ## Installation 📦
 `semchunk` may be installed with `pip`:
@@ -64,15 +65,15 @@
           semchunk.chunkerify(AutoTokenizer.from_pretrained('umarbutler/emubert'), chunk_size) or \
           semchunk.chunkerify(tiktoken.encoding_for_model('gpt-4'), chunk_size) or \
           semchunk.chunkerify(lambda text: len(text.split()), chunk_size)
 
 # The resulting `chunker` can take and chunk a single text or a list of texts, returning a list of
 # chunks or a list of lists of chunks, respectively.
 assert chunker(text) == ['The quick', 'brown', 'fox', 'jumps', 'over the', 'lazy', 'dog.']
-assert chunker([text]) == [['The quick', 'brown', 'fox', 'jumps', 'over the', 'lazy', 'dog.']]
+assert chunker([text], progress = True) == [['The quick', 'brown', 'fox', 'jumps', 'over the', 'lazy', 'dog.']]
 ```
 
 ### Chunkerify
 ```python
 def chunkerify(
     tokenizer_or_token_counter: str | tiktoken.Encoding | transformers.PreTrainedTokenizer | \
                                 tokenizers.Tokenizer | Callable[[str], int],
@@ -88,15 +89,15 @@
 
 `chunk_size` is the maximum number of tokens a chunk may contain. It defaults to `None` in which case it will be set to the same value as the tokenizer's `model_max_length` attribute (deducted by the number of tokens returned by attempting to tokenize an empty string) if possible otherwise a `ValueError` will be raised.
 
 `max_token_chars` is the maximum numbers of characters a token may contain. It is used to significantly speed up the token counting of long inputs. It defaults to `None` in which case it will either not be used or will, if possible, be set to the numbers of characters in the longest token in the tokenizer's vocabulary as determined by the `token_byte_values` or `get_vocab` methods.
 
 `memoize` flags whether to memoize the token counter. It defaults to `True`.
 
-This function returns a callable that takes either a single text or a sequence of texts and returns, if a single text has been provided, a list of chunks up to `chunk_size`-tokens-long with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts.
+This function returns a callable that takes either a single text or a sequence of texts and returns, if a single text has been provided, a list of chunks up to `chunk_size`-tokens-long with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts. The callable can also be passed a `progress` argument which if set to `True` and multiple texts are passed, will display a progress bar.
 
 ### Chunk
 ```python
 def chunk(
     text: str,
     chunk_size: int,
     token_counter: Callable,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: semchunk Version: 0.3.2 Summary: A fast and
+Metadata-Version: 2.3 Name: semchunk Version: 1.0.0 Summary: A fast and
 lightweight pure Python library for splitting text into semantically meaningful
 chunks. Project-URL: Homepage, https://github.com/umarbutler/semchunk Project-
 URL: Documentation, https://github.com/umarbutler/semchunk/blob/main/README.md
 Project-URL: Issues, https://github.com/umarbutler/semchunk/issues Project-URL:
 Source, https://github.com/umarbutler/semchunk Author-email: Umar Butler
 umar.au> License: MIT License-File: LICENCE Keywords:
 chunk,chunker,chunking,chunks,nlp,split,splits,splitter,splitting,text
@@ -14,23 +14,23 @@
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
 Language :: Python :: 3.13 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Classifier: Topic :: Text Processing :: General Classifier:
-Topic :: Utilities Classifier: Typing :: Typed Requires-Python: >=3.9
-Description-Content-Type: text/markdown # semchunk _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_p_y_p_i_/_v_/_s_e_m_c_h_u_n_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/
-_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_/_c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_c_o_v_/_c_/
-_g_i_t_h_u_b_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_]`semchunk` is a fast and lightweight pure Python
-library for splitting text into semantically meaningful chunks. Owing to its
-complex yet highly efficient chunking algorithm, `semchunk` is both more
-semantically accurate than
-[`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://
+Topic :: Utilities Classifier: Typing :: Typed Requires-Python: >=3.9 Requires-
+Dist: tqdm Description-Content-Type: text/markdown # semchunk _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_s_e_m_c_h_u_n_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/
+_s_t_a_t_u_s_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_/_c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_c_o_v_/
+_c_/_g_i_t_h_u_b_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
+_s_e_m_c_h_u_n_k_]`semchunk` is a fast and lightweight pure Python library for splitting
+text into semantically meaningful chunks. Owing to its complex yet highly
+efficient chunking algorithm, `semchunk` is both more semantically accurate
+than [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://
 python.langchain.com/docs/modules/data_connection/document_transformers/
 text_splitters/recursive_text_splitter) (see [How It Works ð](https://
 github.com/umarbutler/semchunk#how-it-works-)) and is also over 90% faster than
 [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/)
 (see the [Benchmarks ð](https://github.com/umarbutler/semchunk#benchmarks-
 )). ## Installation ð¦ `semchunk` may be installed with `pip`: ```bash pip
 install semchunk ``` ## Usage ð©âð» The code snippet below demonstrates
@@ -48,25 +48,25 @@
 ('gpt-4', chunk_size) or \ semchunk.chunkerify('cl100k_base', chunk_size) or \
 semchunk.chunkerify(AutoTokenizer.from_pretrained('umarbutler/emubert'),
 chunk_size) or \ semchunk.chunkerify(tiktoken.encoding_for_model('gpt-4'),
 chunk_size) or \ semchunk.chunkerify(lambda text: len(text.split()),
 chunk_size) # The resulting `chunker` can take and chunk a single text or a
 list of texts, returning a list of # chunks or a list of lists of chunks,
 respectively. assert chunker(text) == ['The quick', 'brown', 'fox', 'jumps',
-'over the', 'lazy', 'dog.'] assert chunker([text]) == [['The quick', 'brown',
-'fox', 'jumps', 'over the', 'lazy', 'dog.']] ``` ### Chunkerify ```python def
-chunkerify( tokenizer_or_token_counter: str | tiktoken.Encoding |
-transformers.PreTrainedTokenizer | \ tokenizers.Tokenizer | Callable[[str],
-int], chunk_size: int = None, max_token_chars: int = None, memoize: bool =
-True, ) -> Callable[[str | Sequence[str]], list[str] | list[list[str]]]: ```
-`chunkerify()` constructs a chunker that splits one or more texts into
-semantically meaningful chunks of a specified size as determined by the
-provided tokenizer or token counter. `tokenizer_or_token_counter` is either:
-the name of a `tiktoken` or `transformers` tokenizer (with priority given to
-the former); a tokenizer that possesses an `encode` attribute (eg, a
+'over the', 'lazy', 'dog.'] assert chunker([text], progress = True) == [['The
+quick', 'brown', 'fox', 'jumps', 'over the', 'lazy', 'dog.']] ``` ###
+Chunkerify ```python def chunkerify( tokenizer_or_token_counter: str |
+tiktoken.Encoding | transformers.PreTrainedTokenizer | \ tokenizers.Tokenizer |
+Callable[[str], int], chunk_size: int = None, max_token_chars: int = None,
+memoize: bool = True, ) -> Callable[[str | Sequence[str]], list[str] | list
+[list[str]]]: ``` `chunkerify()` constructs a chunker that splits one or more
+texts into semantically meaningful chunks of a specified size as determined by
+the provided tokenizer or token counter. `tokenizer_or_token_counter` is
+either: the name of a `tiktoken` or `transformers` tokenizer (with priority
+given to the former); a tokenizer that possesses an `encode` attribute (eg, a
 `tiktoken`, `transformers` or `tokenizers` tokenizer); or a token counter that
 returns the number of tokens in a input. `chunk_size` is the maximum number of
 tokens a chunk may contain. It defaults to `None` in which case it will be set
 to the same value as the tokenizer's `model_max_length` attribute (deducted by
 the number of tokens returned by attempting to tokenize an empty string) if
 possible otherwise a `ValueError` will be raised. `max_token_chars` is the
 maximum numbers of characters a token may contain. It is used to significantly
@@ -75,46 +75,48 @@
 characters in the longest token in the tokenizer's vocabulary as determined by
 the `token_byte_values` or `get_vocab` methods. `memoize` flags whether to
 memoize the token counter. It defaults to `True`. This function returns a
 callable that takes either a single text or a sequence of texts and returns, if
 a single text has been provided, a list of chunks up to `chunk_size`-tokens-
 long with any whitespace used to split the text removed, or, if multiple texts
 have been provided, a list of lists of chunks, with each inner list
-corresponding to the chunks of one of the provided input texts. ### Chunk
-```python def chunk( text: str, chunk_size: int, token_counter: Callable,
-memoize: bool = True, ) -> list[str] ``` `chunk()` splits a text into
-semantically meaningful chunks of a specified size as determined by the
-provided token counter. `text` is the text to be chunked. `chunk_size` is the
-maximum number of tokens a chunk may contain. `token_counter` is a callable
-that takes a string and returns the number of tokens in it. `memoize` flags
-whether to memoize the token counter. It defaults to `True`. This function
-returns a list of chunks up to `chunk_size`-tokens-long, with any whitespace
-used to split the text removed. ## How It Works ð `semchunk` works by
-recursively splitting texts until all resulting chunks are equal to or less
-than a specified chunk size. In particular, it: 1. Splits text using the most
-semantically meaningful splitter possible; 1. Recursively splits the resulting
-chunks until a set of chunks equal to or less than the specified chunk size is
-produced; 1. Merges any chunks that are under the chunk size back together
-until the chunk size is reached; and 1. Reattaches any non-whitespace splitters
-back to the ends of chunks barring the final chunk if doing so does not bring
-chunks over the chunk size, otherwise adds non-whitespace splitters as their
-own chunks. To ensure that chunks are as semantically meaningful as possible,
-`semchunk` uses the following splitters, in order of precedence: 1. The largest
-sequence of newlines (`\n`) and/or carriage returns (`\r`); 1. The largest
-sequence of tabs; 1. The largest sequence of whitespace characters (as defined
-by regex's `\s` character class); 1. Sentence terminators (`.`, `?`, `!` and
-`*`); 1. Clause separators (`;`, `,`, `(`, `)`, `[`, `]`, `â`, `â`, `â`,
-`â`, `'`, `"` and `` ` ``); 1. Sentence interrupters (`:`, `â` and `â¦`);
-1. Word joiners (`/`, `\`, `â`, `&` and `-`); and 1. All other characters.
-`semchunk` also relies on memoization to cache the results of token counters
-and the `chunk()` function, thereby improving performance. ## Benchmarks ð
-On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it
-takes `semchunk` 8.34 seconds to split every sample in [NLTK's Gutenberg
-Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-
-token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18
-texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`]
-(https://pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the
-same texts into 512-token-long chunks â a difference of 92.84%. The code used
-to benchmark `semchunk` and `semantic-text-splitter` is available [here](https:
-//github.com/umarbutler/semchunk/blob/main/tests/bench.py). ## Licence ð
-This library is licensed under the [MIT License](https://github.com/umarbutler/
+corresponding to the chunks of one of the provided input texts. The callable
+can also be passed a `progress` argument which if set to `True` and multiple
+texts are passed, will display a progress bar. ### Chunk ```python def chunk
+( text: str, chunk_size: int, token_counter: Callable, memoize: bool = True, )
+-> list[str] ``` `chunk()` splits a text into semantically meaningful chunks of
+a specified size as determined by the provided token counter. `text` is the
+text to be chunked. `chunk_size` is the maximum number of tokens a chunk may
+contain. `token_counter` is a callable that takes a string and returns the
+number of tokens in it. `memoize` flags whether to memoize the token counter.
+It defaults to `True`. This function returns a list of chunks up to
+`chunk_size`-tokens-long, with any whitespace used to split the text removed.
+## How It Works ð `semchunk` works by recursively splitting texts until all
+resulting chunks are equal to or less than a specified chunk size. In
+particular, it: 1. Splits text using the most semantically meaningful splitter
+possible; 1. Recursively splits the resulting chunks until a set of chunks
+equal to or less than the specified chunk size is produced; 1. Merges any
+chunks that are under the chunk size back together until the chunk size is
+reached; and 1. Reattaches any non-whitespace splitters back to the ends of
+chunks barring the final chunk if doing so does not bring chunks over the chunk
+size, otherwise adds non-whitespace splitters as their own chunks. To ensure
+that chunks are as semantically meaningful as possible, `semchunk` uses the
+following splitters, in order of precedence: 1. The largest sequence of
+newlines (`\n`) and/or carriage returns (`\r`); 1. The largest sequence of
+tabs; 1. The largest sequence of whitespace characters (as defined by regex's
+`\s` character class); 1. Sentence terminators (`.`, `?`, `!` and `*`); 1.
+Clause separators (`;`, `,`, `(`, `)`, `[`, `]`, `â`, `â`, `â`, `â`,
+`'`, `"` and `` ` ``); 1. Sentence interrupters (`:`, `â` and `â¦`); 1. Word
+joiners (`/`, `\`, `â`, `&` and `-`); and 1. All other characters. `semchunk`
+also relies on memoization to cache the results of token counters and the
+`chunk()` function, thereby improving performance. ## Benchmarks ð On a
+desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it takes
+`semchunk` 8.34 seconds to split every sample in [NLTK's Gutenberg Corpus]
+(https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long
+chunks with GPT-4's tokenizer (for context, the Corpus contains 18 texts and
+3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://
+pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the same
+texts into 512-token-long chunks â a difference of 92.84%. The code used to
+benchmark `semchunk` and `semantic-text-splitter` is available [here](https://
+github.com/umarbutler/semchunk/blob/main/tests/bench.py). ## Licence ð This
+library is licensed under the [MIT License](https://github.com/umarbutler/
 semchunk/blob/main/LICENCE).
```

