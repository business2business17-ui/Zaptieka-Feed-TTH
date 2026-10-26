# DE Feed: недостающие позиции из UK (без парентов)

**Файл для загрузки:** `DE_FEED_UPLOAD_19SKU.xlsm` (шаблон `DEUTSCH SKIN_CLEANING_AGENT_SUNSCREEN_EDIBLE_OIL_VEGETABLE_ASTRINGENT_SUBSTANCE_SKIN_MOISTURIZER.xlsm`, строки 7-25, все SKU самостоятельные).
Тексты, INCI, вес, статусы: `DE_SEO_Texte_Missing_Positions.xlsx` (цены на листе «Übersicht» пересчитаны по 1.19).

Параметры (решение владельца): цена EUR = цена UK в GBP × 1.19; количество по 2; сертификаты загружаются отдельно в Account Health. Операция «Erstellen oder Ersetzen (Vollständige Aktualisierung)», ASIN как у живых DE-листингов. ТТХ из Google-таблицы (лист `UK`).

## Что учесть
- **`H3-5FMC-FAD4`, `GO-HRO6-WM8V` (масла)**: пищевые, нужны сертификаты/анализ и этикетка по LMIV (Nährwerttabelle, MHD, ответственный в ЕС). Для рукколы в списке «Zutaten» шаблона нет значения, поле пусто; масло Eruca sativa содержит много эруковой кислоты (пределы в еде: VO (EU) 2019/1870), в Account Health нужен соответствующий анализ.
- **SPF `B8-S7B1-XUBY`**: LSF 50+ / UVA-UVB подтверждаются протоколом испытаний и CPNP.
- Гидролат: «Form des Artikels» и «Duft» пусты (нет подходящих значений в списках). Haaröl/Haarspülung: Browse Node пуст (для SHAMPOO только «Shampoos»).
- `BF-UJUW-N586`: в ТТХ состав (6 масел) расходится с «Преимуществами» (7 масел), использован состав.
- Неактивные на UK SKU (`2L-CFOT-WAF5`, `N4-FRNJ-Q53V`, `R1-RAXF-Z5I9`, `WJ-9EH3-NUHN`) включены по решению владельца.

## Проверки
Dry run 0 FAIL, patch + workbook guard PASS, все обязательные поля заполнены, все значения-списки совпадают со списками шаблона. Заявления уровня «Stufe 1» из ТТХ (лечебные, запрещённые) в тексты не перенесены. Объёмы поиска Cerebro/Helium 10 по новым товарам не сверялись. Загрузку в Amazon не проверял.
