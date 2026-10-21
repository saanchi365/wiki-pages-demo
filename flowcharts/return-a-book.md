# Flowchart – Return a book

*Made-up content for the Shelfie demo.* Based on use cases 3 and 4, and issues #3, #4.

```mermaid
flowchart TD
    a("Reminder: book due in 2 days")
    b{"Want more time?"}
    c{"Someone else reserved it?"}
    d["Renew for 3 more weeks"]
    e["Explain it can't be renewed"]
    f["Return the book at any branch"]
    g("Loan closed")

    a --> b
    b -->|Yes| c
    c -->|No| d --> a
    c -->|Yes| e --> f
    b -->|No| f
    f --> g
```
