# TaskGlitch – SDE Bug Fix Assignment

## Overview

TaskGlitch is a task management web application designed to help sales teams track and prioritize tasks based on ROI (Return on Investment).  
This repository contains my submission for the **SDE Round 1 Bug Fix Assignment**, focusing on identifying and resolving existing issues in a real-world codebase.

---

## Bugs Fixed

1. **Double Fetch on Initial Load**  
   Removed a redundant data fetch that caused duplicate task loading on page refresh.

2. **Undo Snackbar State Bug**  
   Fixed stale undo behavior by resetting the deleted task state when the snackbar closes.

3. **Unstable Task Sorting**  
   Stabilized task sorting by adding a deterministic tie-breaker when ROI and priority match.

4. **Multiple Dialogs Opening**  
   Prevented event bubbling from action buttons to avoid opening multiple dialogs simultaneously.

5. **ROI Calculation Errors**  
   Added proper validation to prevent `NaN` and `Infinity` values during ROI computation.

---

## Tech Stack

- React
- TypeScript
- Vite
- Material UI (MUI)

---

## Live Demo

🔗 **Deployed App:**  
https://task-glitch-poojesh.vercel.app/

---

## Repository

🔗 **GitHub:**  
https://github.com/poojesh-7/task-glitch

---

## Notes

- All fixes are committed with clear, incremental commit history.
- No backend is used; data is handled in-memory as per the original design.
- The app is fully functional and publicly accessible via the deployed link.
