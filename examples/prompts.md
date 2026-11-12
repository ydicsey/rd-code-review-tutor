# Example prompts / 範例指令

## Legacy code / 理解舊程式碼

> EXPLORE mode. Help me understand `LoadNtApi()` in the code I provide. Trace the call flow and explain why `GetProcAddress` is used. Separate confirmed facts from assumptions. Don't run code.

> 使用 EXPLORE 模式：幫我理解 Windows Minifilter 的 PreCreate、PostCreate 與 Cleanup，引用實際程式碼，並說明還需要看哪些檔案才能確認流程。

## Review / 程式碼審查

> REVIEW mode. Review only the attached diff for error handling, race conditions, and backward compatibility. Include P0–P3, evidence, trigger conditions and tests. No edits.

> 使用 REVIEW 模式：先找出經證實的問題，再列出值得確認的假設，不要用通用 checklist 假裝發現 Bug。

## Tutoring / 蘇格拉底式教學

> LEARN mode. Teach me C++ resource lifetime from this repository. Do a short diagnostic, one question per turn, and track my learning.

> 切換 LEARN 模式，教我理解這段 callback 的狀態變化。若我連續兩次答不出來，請直接解釋再換題驗證。
