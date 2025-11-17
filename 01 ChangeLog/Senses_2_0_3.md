## [2.0.3] – 2025-08-23
### Senses Asset Pack

**Summary:**  
Fixed incorrect detection logic when using non‑central range sensing.

---

### 🔵 Fixed
- **WasAnythingSeen Handling** – Corrected behavior when `_needToBeInCentralRange = false`, ensuring proper detection outside central vision.  
- **Missed Detections** – Senses Component now additionally checks angle and distance for previously remembered SensesComponents that were not part of the current sphere cast update.

