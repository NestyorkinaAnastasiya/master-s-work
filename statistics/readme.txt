каждые 5 минут собирается информация с очереди СУПЗ в файл qtatinfo.json
после чего запускается python.py, где собирается информация с qtatinfo.csv в виде словаря:
{
id задачи: {
	количество узлов: ,
	количество потоков: ,
	walltime: ,
	время ожидания в очереди СУПЗ: ,
	время выполнения задачи:
}...
}, далее информация обновляется с учётом qtatinfo.json (добавляются новые задачи, обновляются старые)
после чего данные перезаписываются в qtatinfo.csv