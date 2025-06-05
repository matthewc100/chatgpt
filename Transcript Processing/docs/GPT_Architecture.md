# GPT Architecture

This document outlines the functional design of the Transcript Formatter GPT.

## Components
- Transcript Cleaner
- Speaker Aggregator
- Format Converter
- Optional Summary Generator

## Flow
1. Ingest VTT or plain text transcript.
2. Strip timestamps and numeric markers.
3. Aggregate dialogue per speaker.
4. Format based on selected output.
5. Optionally add Summary, Action Items, and Meeting Details.
