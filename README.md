Первоначально код загружает данные из CSV-файла, который находится по указанной ссылке. 

Затем выполняется очистка текста, с помощью функции clean_text. 

В этой функции используются регулярные выражения для удаления ненужных элементов текста, таких как временные метки, 
веб-ссылки и специальные символы. Это помогает создать более структурированный и однозначный текст, 
который может служить основой для последующего анализа или генерирования задач.
Далее делал различную токенизацию по очищенному тексту, но никаких значимых результатов не дало(из кода удалил).

Одним из самых важных шагов является генерация задач на основе очищенных диалогов с использованием модели для 
обработки естественного языка.

После генерации задач, код также включает функцию remove_duplicate_tasks, которая предназначена для удаления 
дубликатов среди сгенерированных задач. Это решает проблемы с повторяющимися или схожими задачами, что в свою 
очередь способствует более четкому и организованному представлению информации.

Вывод результатов в конце кода демонстрирует, как были сформированы сгенерированные задачи для каждого диалога. 
Это заключительный этап обработки, который показывает соответствие заданным критериям и позволяет оценить 
результат с точки зрения актуальности и полезности задач.
