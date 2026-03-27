
---

### **SQL-ГАЙД (sql-guide)**

```markdown
# 📚 SQL Window Functions Guide

**Проект:** Гайд по оконным функциям SQL: ROW_NUMBER, RANK, DENSE_RANK  
**Автор:** GlebShalunkov  
**Технологии:** SQL, Python, Pandas

## 📌 О проекте
Практическое руководство с примерами на Python и SQL.

## 🎯 Что внутри
- Турнирная таблица: разница между функциями
- Клиентский анализ: рейтинг по сумме заказов
- SQL-запросы и Pandas-аналоги
- Когда что использовать

## 🔥 Примеры
```sql
SELECT 
    player_name,
    score,
    ROW_NUMBER() OVER (ORDER BY score DESC) as row_num,
    RANK() OVER (ORDER BY score DESC) as rank_num,
    DENSE_RANK() OVER (ORDER BY score DESC) as dense_rank
FROM players;
