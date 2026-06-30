
---

## PPT-Master (июнь 2026)

**Репозиторий:** `~/ppt-master/` (клон `github.com/hugohe3/ppt-master`, v2.11.0, MIT)  
**Автор:** Hugo He (Китай, CPA/CPV/консультант по инвестициям)  
**Назначение:** AI-генерируемые нативные PPTX из любого документа

**Вход:** PDF, DOCX, XLSX, Markdown, URL, PPTX  
**Выход:** Редактируемый `.pptx` с DrawingML-шейпами, анимациями, аудионаррацией speaker notes

**Установка:** `~/ppt-master/.venv/` (Python 3.11, все зависимости)  
**Активация:** `source ~/ppt-master/.venv/bin/activate`

**Конвертеры источников:**
- `pdf_to_md.py` → PDF → Markdown (PyMuPDF)
- `doc_to_md.py` → DOCX/HTML/EPUB → MD (mammoth)
- `excel_to_md.py` → XLSX → MD (openpyxl)
- `web_to_md.py` → URL → MD (requests+bs4)
- `ppt_to_md.py` → PPTX → MD

**Работает как skill** для: Claude Code, Cursor, VS Code + Copilot, Codebuddy  
**Стоимость:** ~$0.08/колода (только токены LLM)  
**Ключевая фишка:** не картинки слайдов, а нативные объекты PowerPoint

