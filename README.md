paper’s title:
Arabic calligraphy‑based text steganography framework with biologically‑encoded secret messages, enhanced embedding capacity and automated extraction.
# BioStegoScript

## Overview
BioStegoScript is an Arabic calligraphy-based linguistic steganography framework for concealing secret messages inside visually natural Arabic text segments. The framework combines biological-inspired encryption, Arabic letter-shape variation, Kashida extensions, whitespace variations, and automated CNN-based extraction.

The system first converts the secret message into a biologically encoded encrypted bitstream through DNA, RNA, and protein-symbol mappings. The resulting encrypted bit sequence is then matched against the binary representations of complete Arabic text segments. Each segment can have multiple valid calligraphic forms because Arabic letters may appear in different shapes and positions, and because Kashida and whitespace can be varied while preserving the visible meaning and readability of the segment.

A modified Aho–Corasick matching method, called AC
∗
∗
 , searches for a complete segment whose encoded calligraphic form matches the encrypted secret bits. After a matching segment is found, the Arabic calligrapher or rendering system writes the full segment using the required letter shapes, Kashida placements, and whitespace patterns. The final rendered Arabic segment becomes the stego-text or stego-image.

During extraction, the system identifies the Arabic letter forms, Kashida states, and whitespace patterns, converts them back into the encrypted bitstream, reverses the biological encoding, and recovers the original secret message. The published framework also introduces CNN-based automated extraction to replace manual identification of Arabic calligraphic letter shapes.
## Core Pipeline
Secret message
      ↓
Biological encoding and encryption
      ↓
Encrypted binary bitstream
      ↓
AC* matching against complete encoded Arabic segments
      ↓
Matching Arabic segment with a valid full letter-form sequence
      ↓
Calligraphic rendering:
letter shapes + Kashida + whitespace
      ↓
Stego Arabic text or stego-image
      ↓
CNN-based extraction
      ↓
Recovered encrypted bits
      ↓
Biological decoding
      ↓
Original secret message

## Key Characteristics
Key Characteristics
Uses complete Arabic segments rather than isolated words or characters.

Preserves the semantic meaning of the selected Arabic segment.

Represents hidden data through multiple Arabic letter shapes, Kashida, and whitespace.

Uses a biological-inspired encoding layer before calligraphic embedding.

Uses AC
∗
∗
  to match the complete encrypted bitstream with a complete encoded segment.

Supports automated extraction using a convolutional neural network.

Uses Arabic Naskh calligraphy as the primary rendering environmen
