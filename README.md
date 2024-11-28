# Product-Name-Matching-System
*Solution Overview
->Manual Matching for First-time Entries: The system will allow a user to manually map unknown product names to standardized names.
->Mapping Dictionary Maintenance: Automatically map known variations using a pre-built dictionary.
->Handling Variations: Use string similarity techniques (like Levenshtein distance) to intelligently suggest potential matches.
->Update and Extend Mapping: Allow easy updates to the dictionary for future variations.
*Explanation
 Manual Matching:
   For first-time entries, the user is prompted to input a standardized name.
 Automatic Matching:
   Uses the fuzzywuzzy library to suggest potential matches for unmapped names based on similarity.
 Mapping Dictionary:
   A dictionary is used to store mappings. The dictionary is saved and loaded from a file for persistence.
 Handle New Variations:
   New variations are intelligently handled by suggesting potential matches or allowing manual mapping.
*Assumptions
  Variations in product names are primarily due to spacing, abbreviations, or word order.
  Users will provide valid input when prompted for standardized names.
*Use Cases Handled
  Synonyms or different orders of words in product names.
  Variations in spacing, abbreviations, and casing.
*Future Improvements
  Enhanced Similarity Matching: Incorporate advanced NLP models (e.g., BERT) for more robust name similarity checks.
  Batch Mapping: Allow users to map multiple names at once.
  Web Interface: Provide a user-friendly web interface for managing mappings.
