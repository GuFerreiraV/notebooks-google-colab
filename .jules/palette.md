# Palette's Journal - Critical Learnings Only

## 2025-05-14 - [Adding Progress Feedback to Batch Processing]
**Learning:** For long-running operations in Jupyter Notebooks (like processing multiple images through ML models), providing visual feedback via `tqdm` significantly improves the user experience by indicating progress and preventing the perception of a frozen interface.
**Action:** Always consider wrapping long-running loops in `tqdm` when working on notebooks or CLI tools.
